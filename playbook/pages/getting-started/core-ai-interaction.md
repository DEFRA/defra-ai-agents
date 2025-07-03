## 2.10. Core Interaction Patterns – RAG, Semantic Search & AI Chat

This section introduces three foundational AI interaction patterns commonly used across AI agents, workflows, and user-facing systems:

- **Semantic Search**: Meaning-based content retrieval
- **Retrieval-Augmented Generation (RAG)**: Generating responses grounded in trusted sources
- **AI Chat Interfaces**: Conversational tools for interacting with data, decisions, or services

These are reusable building blocks that support explainability, safety, and usability — and align with the UK Government AI Playbook's principles of modularity, transparency, and public trust.

> ⚠️ These patterns may be used individually or together — but they require additional governance considerations when deployed at scale or for public use.

> **Note:** Any example use cases are to illustrate where Core Interaction Patterns *could* be applied within Defra contexts.  
> They are **not confirmations**


---

### Semantic Search

Semantic search allows users or systems to retrieve relevant information based on meaning rather than keywords. It works by embedding content and queries into a shared vector space and matching based on similarity.

**When to use:**
- To improve discovery across long-form or unstructured data (e.g. policy PDFs, case files)
- As part of a RAG pipeline or intelligent retrieval system

**Example (Defra):**
- A biodiversity enforcement officer searches for similar incident reports by typing “unauthorised tree felling near wetland” — the system finds contextually similar past cases and legislation.

**Best Practices:**
- Use high-quality domain-specific embeddings
- Validate top results regularly
- Provide users with fallback keyword search and filters
- Keep content version-controlled and transparent

---

### Retrieval-Augmented Generation (RAG)

RAG combines semantic search with LLMs. It retrieves trusted documents in response to a query, then feeds them into a prompt to generate a grounded answer. This helps reduce hallucinations and improves explainability.

**When to use:**
- To answer complex questions based on policies, datasets, or knowledge banks
- To support internal or public-facing Q&A agents where source traceability is needed

**Example (Defra):**
- A land use assistant agent receives a query: “Can I build a barn on a floodplain?”  
  The system retrieves policy documents and local risk data, then generates a grounded response citing the relevant source.

**Best Practices:**
- Store and manage source data securely and transparently
- Use fixed context windows or memory where needed
- Annotate LLM outputs with retrieved content references
- Always log retrieval results and final output

---

### AI Chat Interfaces

AI chat allows users to interact with agents, workflows, or knowledge bases through a conversational interface. These are typically built around a core LLM and may include RAG or tool use.

**When to use:**
- To support staff or public users in navigating policies, completing forms, or accessing internal knowledge
- As an interface to complex multi-step agents or workflows

**Example (Defra):**
- A farmer uses a conversational tool to ask questions about pesticide regulations. The system uses RAG and semantic search to retrieve guidance, and presents it through a friendly, transparent chat UI.

**Best Practices:**
- Clearly disclose when users are interacting with an AI
- Provide a human escalation path
- Avoid speculative or open-ended advice (especially legal, health, regulatory)
- Log interactions and user feedback

---

### Summary Table

| Pattern            | Use Case Example                             | Where It Fits                   |
|--------------------|----------------------------------------------|----------------------------------|
| **Semantic Search** | Find similar past enforcement cases          | Knowledge retrieval for staff   |
| **RAG**             | Answer questions using grounded documents    | Internal Q&A, permitting advice |
| **AI Chat**         | Conversational tool for farming subsidies    | Public-facing guidance and support |

---

> 📌 These patterns are modular and can be reused across agents, workflows, and user tools.  
> When used, they must follow Defra’s governance standards and the UK Government AI Playbook’s guidance on safety, transparency, and effectiveness.