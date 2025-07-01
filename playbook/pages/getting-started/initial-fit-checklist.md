## 2.2 Initial Fit Checklist
Use this score-based checklist to evaluate which type of system best fits your use case: AI Agents, AI Workflows, RPA, or Multi-Agent Systems.

> Each question is scored from 0 to 3:
>
> - **0 = Not true**
> - **1 = Partially true**
> - **2 = Mostly true**
> - **3 = Definitely true**

---

### Questions & Scoring

| Question | Score (0–3) | Notes |
|----------|-------------|-------|
| 1. Does the task require autonomous decision-making? |   | E.g. triggering actions based on inputs without human prompts |
| 2. Is the environment dynamic or context-dependent? |   | Does it need to adapt to changing data or goals? |
| 3. Is the task highly repetitive and rule-based? |   | Great candidate for RPA or simple workflows |
| 4. Does the system need to coordinate across roles or domains? |   | Is there collaboration or negotiation across stakeholders? |
| 5. Does the solution require explainability or human auditability? |   | Will humans need to justify, monitor, or override decisions? |

---

### Interpreting the Scores

| System Type               | Indicators |
|---------------------------|------------|
| **AI Agent**              | High score (≥5) across Q1 + Q2 |
| **Traditional Automation (RPA)** | High score (≥2) on Q3, and low scores on Q1, Q2, Q4 |
| **AI Workflow**           | High scores on Q5 (and possibly Q3), especially if model + rule hybrid |
| **Multi-Agent System**    | High score (≥2) on Q4, and Q1/Q2 are also moderately high |

---

### Example Interpretation

| Example Use Case                      | Q1 | Q2 | Q3 | Q4 | Q5 | Likely Fit            |
|--------------------------------------|----|----|----|----|----|------------------------|
| Automating permit data entry         | 0  | 0  | 3  | 0  | 1  | 🟩 Traditional RPA     |
| Monitoring invasive species          | 3  | 3  | 1  | 0  | 2  | 🟦 AI Agent             |
| Policy impact simulation             | 2  | 2  | 1  | 3  | 3  | 🟨 Multi-Agent System   |
| Subsidy eligibility scoring (audited)| 1  | 1  | 2  | 0  | 3  | 🟧 AI Workflow          |

---

### Tips

- If your task is mostly static and structured, start with RPA or an AI Workflow before exploring full AI Agents.
- Multi-Agent Systems should only be considered when there’s real complexity in coordination or simulation.
- AI Workflows are especially valuable when models and rules need to work together in a controlled, auditable process.
- AI Agents add value where automation must respond to changing inputs or goals with minimal human input.

---