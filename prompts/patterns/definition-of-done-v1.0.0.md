# [Pattern] Definition of Done (DoD) Checklist

## Context
Use this pattern at the end of any task to ensure it meets the repository's quality standards before commit.

## Mandatory Checklist
1. **Validation:** Does the output fulfill 100% of the initial prompt requirements?
2. **Naming:** Does the file name follow the `<area>-<capability>-<scope>-vMAJOR.MINOR.PATCH.md` convention?
3. **Sections:** Does it include all required sections (Purpose, Role, Inputs, Instructions, Output Format)?
4. **Clean Code:** If it contains code, does it follow DRY and KISS principles?
5. **Documentation:** Is there a "Learning Tip" or "Example" included for educational purposes?

## Verification Step
The AI must perform a self-audit using this list and explicitly state: "This task is COMPLETED because [reasons]" or "This task is PENDING because [reasons]".