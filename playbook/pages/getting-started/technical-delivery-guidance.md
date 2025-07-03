## 2.6. Technical & Delivery Guidance

This section provides practical guidance for designing, building, testing, and deploying AI agents, workflows, RPA bots, and multi-agent systems within Defra.

> **Note:** Any examples of potential AI tools and framework use (e.g. LangChain, Azure AI Studio, Semantic Kernel, OpenAI Assistants) are illustrative only. Always consult the Defra AI Tools Authority or your technical governance lead before selecting or implementing any AI technology to ensure alignment with internal standards, approved platforms, and procurement policy.

---

### System Architecture Layers

Most intelligent systems can be broken down into four layers:

| Layer              | Description | Applies to |
|-------------------|-------------|------------|
| **Perception (Input)**  | Collects data from APIs, files, sensors, forms, or human input. | All system types |
| **Reasoning (Logic/Model)** | Encodes the rules, models, or goals that determine what the system decides. | AI Agents, AI Workflows, MAS |
| **Action (Execution)**  | Performs actions: updates systems, sends alerts, triggers APIs, etc. | RPA, Agents, Workflows |
| **Feedback/Adaptation** | Captures outcomes or errors to enable learning or improve future responses. | AI Agents, MAS (optional in RPA/Workflows) |

> AI Agents and MAS should be designed with **feedback loops** to adapt based on performance or outcomes.


### Tool Selection & Integration

Use this table to help select Potential tooling/stack for your automation or AI system, including support for RPA, AI agents, multi-agent systems, and orchestration workflows. Selection should always align with the specific use case, risk profile, and existing platform preferences.

| Task / Goal                           | Potencial Tools / Stack |
|---------------------------------------|----------------------------|
| RPA for UI-based automation           | UiPath, Power Automate |
| Multi-step AI workflows               | LangGraph, Microsoft Semantic Kernel |
| Agent development                     | Azure AI Foundary (GPT via OpenAI), Claude Agents (via Bedrock), AutoGen |
| Integration with Defra systems        | RESTful APIs, Microsoft Graph |
| Data pipelines                        | Azure Data Factory, AWS Glue, Pandas for transformation |


### Key Delivery Activities

#### 1. **Design for Governance from the Start**
- Define who is accountable (business owner, product owner)
- Create a deployment plan that includes fail-safes, monitoring, and oversight points

#### 2. **Test Models, Workflows, and Agents Thoroughly**
- Use real data in approved environments
- Define metrics (accuracy, latency, false positive rate, impact)
- Include human-in-the-loop testing for critical decisions

#### 3. **Secure and Document the Data Pipeline**
- Validate data quality, completeness, and bias before training or automation
- Use Defra data standards for consistency
- Store and version datasets and models for audit purposes

#### 4. **Deploy with Monitoring and Alerting**
- Log all actions by agents or bots (inputs, outputs, decisions)
- Set alerts for failures, thresholds breached, or unexpected behaviour
- Use dashboards to support live operations and oversight

#### 5. **Plan for Post-Deployment Learning or Iteration**
- Set regular review cycles for updating models, rules, or behaviours
- Incorporate user feedback mechanisms (especially for internal tools)
- Maintain a change log for governance and improvement tracking

---

### Metrics to Track

| Metric Type      | Examples |
|------------------|----------|
| **Performance**  | Accuracy, latency, coverage, error rate |
| **Impact**       | Time saved, decisions accelerated, consistency improvements |
| **Fairness**     | Outcome parity across demographics or regions |
| **Transparency** | % of decisions logged with justification; ATRS completed |
| **Safety**       | Number of errors detected; time to detect/respond to anomalies |


### Security & Access Control

- Implement role-based access for dashboards, models, and workflows
- Encrypt sensitive inputs/outputs (e.g. personal or environmental data)
- Ensure audit logging is in place for any decisions affecting citizens or the environment
- Follow Defra and CDDO guidance on secure deployment and monitoring

> Refer to: [Gov UK AI Playbook – Build and Test](https://www.gov.uk/government/publications/ai-playbook-for-the-uk-government)

---

### Best Practices by System Type

| System Type          | Build & Delivery Tips |
|----------------------|-----------------------|
| **AI Agents**        | Use goal-driven design, clearly define perception/action boundaries, log decisions and actions. |
| **AI Workflows**     | Chain together decision points with checkpoints, use rule engines or ML models, design for auditability. |
| **Traditional RPA**  | Script simple, repeatable tasks. Avoid embedding business logic that changes often. Use error handling and dashboards. |
| **Multi-Agent Systems** | Test agent roles independently, simulate interactions, define conflict resolution mechanisms. Monitor emergent behaviour. |
