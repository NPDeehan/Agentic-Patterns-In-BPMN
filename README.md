# 🧠 Agentic Patterns in BPMN

This project demonstrates how to implement **Agentic Patterns** using **BPMN** (Business Process Model and Notation), a standard for modeling business processes. These patterns showcase how intelligent agents can be orchestrated and structured visually using BPMN elements.

## ✨ Featured Patterns

### 🔁 ReAct Pattern (Reason + Act)
Combines reasoning and action steps in a loop. The agent reflects before acting and adapts based on new information. In BPMN, this is modeled with looping flows between reasoning tasks and action tasks.

![React](./img/1.%20Reasoning%20&%20Acting%20Agent.png)

**Use case**: Iteratively solving tasks using LLM reasoning and external tool invocations.

---

### 🛠️ Modern Tool Pattern
Agents leverage specialized external tools (e.g., APIs, vector stores) rather than trying to solve everything themselves. BPMN allows clear orchestration of these calls as service tasks.

![modTool](./img/2.%20Modern%20Tool%20Use.png)

**Use case**: Tool-augmented reasoning with LLMs calling APIs or databases.

---

### 🪞 Self-Reflection Pattern
Agents periodically pause to evaluate or critique their own reasoning or outputs. BPMN models this using gateways and evaluation subprocesses to decide whether to continue or revise the plan.

![selfRef](./img/4.%20Agent%20Self-Reflection.png)

**Use case**: Agents revisiting previous steps to identify and correct mistakes.

---

### 📚 RAG Pattern (Retrieval-Augmented Generation)
Incorporates external knowledge into the agent’s reasoning process by retrieving relevant documents or data before generating responses. Modeled in BPMN by:
- A **service task** to query a knowledge base or vector store.
- A subsequent **script or LLM call** using the retrieved context.

![ragAgent](./img/3.%20Agentic%20Retrieval-Augmented%20Generation.png)

**Use case**: Answering questions using up-to-date or domain-specific knowledge without retraining the model.

---

### 👥 Multi-Agent Pattern
Multiple agents collaborate or compete to solve a problem. BPMN supports this through message flows between separate participants (pools), with synchronization points.

![multiTool](./img/5.%20Multi-Agent%20Workflow.png)

**Use case**: Planner, executor, and critic agents coordinating on a shared task.

---

### 👤 Human-in-the-Loop Pattern
Critical decision points are handed off to humans for input, validation, or override. In BPMN, this is represented with user tasks.

![humanLoop](./img/6.%20Human%20in%20the%20Loop.png)

**Use case**: Human approval of AI-generated responses or plans.

---

### ⏳ Long-Running Agentic Orchestrations
Agentic workflows that span hours or days, waiting for external events or conditions. BPMN models this using timer events, message events, and intermediate states.

![longRun](./img/7.%20Long%20Running%20Agentic%20Orchestration.png)

**Use case**: Agents triggered by data changes, user actions, or scheduled checks.

---


