# Playbook: Designing Agentic Solutions in Enterprise Architecture

## Introduction
This playbook provides a step-by-step guide to positioning AI Agents within a TOGAF or ArchiMate framework. It ensures that "Agentic" solutions are not just standalone scripts but integrated components of the Enterprise Architecture.

## Prerequisites
- Access to an LLM (ChatGPT, Gemini, or Copilot).
- The `dev-arch-doc-v1.0.0.md` prompt from this repository.

---

## 🟢 Level 1: Basic Execution (Fast Track)
*Ideal for quick prototyping and non-technical stakeholders.*

### Step 1: Context Gathering
Identify the "Agent's Territory". Ask yourself: 
- What specific task will the agent perform? (e.g., "Summarize emails").
- What info does it need to read? (e.g., "Access to Outlook").

### Step 2: Running the Prompt
Copy the content of `prompts/roles/developer/dev-arch-doc-v1.0.0.md` and provide simple inputs:
- **Problem Statement:** Describe your manual task.
- **Agent Capabilities:** Describe what the AI should do (Read, Write, Analyze).

### Step 3: Basic Validation
- Does the output solve the immediate problem?
- Is the tone and format correct for your team?

---

## 🔵 Level 2: Advanced Execution (Architect Level)
*Ideal for integrating AI into Enterprise Frameworks (TOGAF/ArchiMate).*

### Step 1: Pattern Injection (The "Secret Sauce")
Before running the main prompt, "prime" the AI with the **System Architect Pattern**:
1. Open `prompts/patterns/system-architect-pattern-v1.0.0.md`.
2. Paste it into your LLM. This forces the AI to reason through Business, Application, and Technology layers.

### Step 2: Technical Mapping
Provide specific architectural context:
- **Current Framework:** Mention the specific TOGAF ADM Phase (e.g., Phase C: Information Systems Architectures).
- **Constraints:** Include Data Sovereignty, API limits, and Security protocols.

### Step 3: Modeling in ArchiMate
Use the prompt output to create formal diagrams. 

- **Modeling Rule:** Represent the AI Agent as an **Application Function** assigned to an **Application Component**.
- **Relationships:** Use "Serving" or "Access" relationships to show how the agent interacts with Data Objects.

---

## 🛠️ Troubleshooting & Tips
- **Output is too generic:** Provide more details about the existing integration points (APIs, Databases).
- **Hallucinations:** Ask the AI to cite specific TOGAF ADM principles to ground its reasoning.
- **Governance:** Always ensure the output matches the `required_sections` defined in our `catalog.yaml`.