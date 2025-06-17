## ✅ AI System Selection Checklists

Use the following checklists to help determine which automation or AI approach best fits your use case.

Each question includes a simple example relevant to Defra to help guide your answers.

---

### 🤖 AI Agent Checklist

Tick the boxes if the statement applies to your use case:

- [ ] Does the system need to make autonomous, goal-driven decisions?  
  _Example: An agent that detects invasive species and triggers mitigation actions based on risk level._

- [ ] Will it operate in a dynamic or unpredictable environment?  
  _Example: An agent adjusting flood risk assessments in real time as weather and water level data changes._

- [ ] Will it act on real-time inputs (e.g. sensors, live feeds)?  
  _Example: Monitoring air quality data and issuing alerts if thresholds are breached._

- [ ] Should it be able to adapt or improve over time?  
  _Example: An agent that learns and refines patterns of illegal waste dumping from drone footage._

- [ ] Is low-latency, high-frequency decision-making important?  
  _Example: An autonomous irrigation agent that quickly reacts to soil moisture sensors to avoid crop stress._

✅ **If you ticked 3 or more, an AI Agent may be suitable.**

---

### 🔁 AI Workflow Checklist

Tick the boxes if the statement applies:

- [ ] Is the task rule-based or follows a repeatable, structured process?  
  _Example: Processing agricultural subsidy applications through a set of eligibility checks._

- [ ] Do you need to chain multiple models or rules together?  
  _Example: A pipeline that classifies satellite imagery, scores ecological impact, and routes to a reviewer._

- [ ] Is a human decision-maker needed for validation or oversight?  
  _Example: An AI suggests land use changes, but planners must approve the final output._

- [ ] Is a record of decisions or steps required for audit purposes?  
  _Example: A permit decision workflow that must log each scoring step for transparency._

- [ ] Is compliance with regulatory or legal processes critical?  
  _Example: Environmental compliance checks that require both AI assistance and full traceability._

✅ **If you ticked 3 or more, consider using an AI Workflow.**

---

### 🤖 Traditional Automation (RPA) Checklist

Tick the boxes if the statement applies:

- [ ] Is the task repetitive and rules-based with minimal variation?  
  _Example: Downloading monthly farm inspection reports from a web portal._

- [ ] Does it involve interacting with existing software systems via UI (e.g. data entry)?  
  _Example: Copying values from a government spreadsheet into a legacy application with no API._

- [ ] Can the logic be fully scripted with no need for machine learning or real-time inputs?  
  _Example: Sending a fixed-format weekly report to multiple stakeholders._

- [ ] Is it primarily about increasing processing speed or reducing human error?  
  _Example: Automating manual data entry to reduce copy-paste mistakes._

- [ ] Would a macro or script solve the problem, but you want it to scale?  
  _Example: A bot that processes hundreds of similar permit renewals per week._

✅ **If you ticked 3 or more, RPA may be the best fit.**

---

### 🤝 Multi-Agent System Checklist

Tick the boxes if the statement applies:

- [ ] Are multiple autonomous roles or perspectives involved?  
  _Example: A model where agents represent farmers, regulators, and conservationists in land-use decisions._

- [ ] Is there a need for coordination, negotiation, or cooperation between actors?  
  _Example: Simulating the response of emergency services and utilities during a major flood event._

- [ ] Does each role require its own decision logic or model?  
  _Example: One agent forecasts water demand; another controls reservoir levels; a third plans crop rotation._

- [ ] Is the problem decentralised or distributed across teams, domains, or geographies?  
  _Example: A national wildfire model where each region's response is governed by separate agent rules._

- [ ] Would simulation of stakeholder behaviour be valuable?  
  _Example: Testing how different land management policies might affect farming output and biodiversity._

✅ **If you ticked 3 or more, a Multi-Agent System may be appropriate.**

---

### 📌 Tip

You can combine approaches:

- **RPA** may trigger **AI Workflows**
- **AI Agents** can operate inside or alongside **Workflows**
- **Multi-Agent Systems** may include agents powered by AI or RPA

Start with the simplest tool that meets your need and scale in complexity only as needed.