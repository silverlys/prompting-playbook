# Playbook: Modern Development Best Practices

## Introduction
This playbook establishes the technical excellence standards for this repository. Its goal is to ensure that every piece of code is maintainable, scalable, and follows professional engineering principles.

---

## 🟢 1. The Clean Code Foundation
Writing code that "works" is not enough; it must be readable for humans.
- **Meaningful Names:** Use intention-revealing names for variables and functions (e.g., `calculate_total_price` instead of `calc`).
- **Function Size:** Keep functions small. If a function does more than one thing, split it.
- **Comments Policy:** Use comments only to explain "Why" (intent), not "What" (the code should explain itself).

## 🔵 2. Modern Git Workflow
A clean repository is as important as clean code.
- **Atomic Commits:** Each commit should solve one specific thing. 
- **Standard Messages:** Use the Conventional Commits format (`feat:`, `fix:`, `docs:`, `refactor:`).
- **Clean History:** Avoid pushing temporary files or environment secrets (enforced by our `.gitignore`).

## 🟡 3. Architectural Thinking
Before coding, define the structure to avoid "Spaghetti Code".
- **SoC (Separation of Concerns):** Keep your Business Logic separate from your Data Access and UI layers.
- **SOLID Principles:** - *Single Responsibility:* One class, one purpose.
    - *Open/Closed:* Software entities should be open for extension but closed for modification.
- **Pattern Usage:** Always "prime" the AI with the `system-architect-pattern` before generating new modules.

## 🔴 4. Security & Performance
- **Zero Trust with Secrets:** Never hardcode API keys or passwords. Use environment variables.
- **Input Validation:** Never trust external data. Sanitize all inputs before processing.
- **YAGNI (You Ain't Gonna Need It):** Don't build features or complex architectures until they are actually necessary.

---

## ✅ The "Definition of Done" (DoD)
A development task is considered **Done** only when:
1. The code has been refactored using the `dev-clean-code-refactor` prompt.
2. It has been audited by the `dev-best-practices-reviewer`.
3. The file naming convention follows the repository governance.
4. No "Dead Code" or unused dependencies remain.
## 🧩 Practical Application: The "Sandwich" Technique

To get a professional-grade audit that helps you refresh your knowledge, follow this execution sequence in your AI assistant:

1. **The Foundation (Pattern):** Paste the content of `prompts/patterns/clean-code-standards-v1.0.0.md`.
2. **The Mindset (Role):** Paste the content of `prompts/roles/developer/dev-reviewer-v1.0.0.md`.
3. **The Subject (Code):** Provide your code snippet for review.

**Why this order?**
- The **Pattern** sets the rules (Clean Code/SOLID).
- The **Role** sets the expertise (Senior Architect).
- The **Code** provides the context.