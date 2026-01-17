# Playbook: Designing Agentic Solutions in Enterprise Architecture

## Introduction
This playbook provides a step-by-step guide to positioning AI Agents within a TOGAF or ArchiMate framework. It ensures that "Agentic" solutions are not just standalone scripts but integrated components of the Enterprise Architecture.

## Prerequisites
- Access to an LLM (ChatGPT, Gemini, or Copilot).
- Basic understanding of ArchiMate layers (Business, Application, Technology).
- The `dev-arch-doc-v1.0.0.md` prompt from this repository.

## Step-by-Step Execution

### Step 1: Context Gathering
Before running the prompt, identify the "Agent's Territory". Ask yourself: 
- Is the agent a **service** (Application Layer) or an **actor** (Business Layer)?
- What data stores will it access?

### Step 2: Running the Prompt
Copy the content of `prompts/roles/developer/dev-arch-doc-v1.0.0.md` and provide the following inputs:
- **Problem Statement:** "Need to automate the PQRS claims triage process."
- **Current Framework:** "Application Architecture layer."
- **Agent Capabilities:** "Language understanding and SQL tool-use."

### Step 3: Validating the Output
Check the AI's response against these criteria:
- **Traceability:** Does the agent's action map back to a business requirement?
- **Constraints:** Are security and ethical boundaries defined for the agent?

### Step 4: Modeling in ArchiMate
Use the "Modeling Suggestions" from the prompt output to create your diagram. 
- *Pro Tip:* Represent the AI Agent as an **Application Function** assigned to an **Application Component**.

## Troubleshooting
- **Output is too generic:** Provide more details about the existing integration points (APIs, Databases).
- **Hallucinations:** Ask the AI to cite specific TOGAF ADM phases to ground the reasoning.
