# [Pattern] Clean Code & SOLID Standards

## Context
Use this pattern when generating, refactoring, or reviewing source code to ensure enterprise-grade quality.

## Principles to Enforce
1. **Meaningful Names:** Variables, functions, and classes must have descriptive names that reveal intent. Avoid abbreviations like `temp` or `data`.
2. **Function Purity:** Each function must do only one thing (Single Responsibility). Functions should ideally not exceed 20 lines of code.
3. **Error Handling:** Use exceptions instead of return codes. Ensure `try-catch` blocks are specific and meaningful.
4. **DRY (Don't Repeat Yourself):** Identify and abstract logic that appears more than once.
5. **KISS (Keep It Simple, Stupid):** Avoid "clever" or over-engineered solutions. Clarity is better than brevity.

## Review Steps
Before providing the final code, the AI must:
- List any principles that were initially violated.
- Explain how the refactored version adheres to these standards.