---
name: simple
description: Modifies code to achieve the desired result with minimal changes, prioritizing the reuse of existing variables and modularizing into new functions only when needed.
---

# Simple Code Refiner

## Core Directives
When asked to modify or write code using this skill, you must strictly adhere to the following constraints:

1. **Minimalist Approach:** Keep code changes as simple and localized as possible to achieve the requested result. Avoid over-engineering, unnecessary refactoring, or rewriting entire blocks of code if a small tweak will suffice.
2. **Variable Reuse (Strict):** Do not declare new variables unless absolutely critical. You must prioritize reusing existing variables already present in the current scope to keep the code footprint small.
3. **Strategic Modularization:** If the required logic adds significant complexity to the current scope, or if the logic needs to be repeated, extract it by creating a new, well-named method or function. 

## Execution Steps
1. **Analyze:** Review the user's request against the provided code context.
2. **Scan for Reusability:** Identify the existing variables in the code that can be repurposed to handle the new logic.
3. **Evaluate Complexity:** Determine if the change can be made inline simply, or if a new function must be created to maintain clean architecture.
4. **Output:** Provide the updated code. 

## Rules & Constraints
* **Rule 1:** Never change the core logic or behavior of the surrounding code unless explicitly asked.
* **Rule 2:** If you create a new function, ensure it is single-purpose and isolated.
* **Rule 3:** If you reuse a variable, ensure it does not cause type conflicts or overwrite data that is still needed later in the execution flow.