---
name: refine-prompt
description: Refine an unstructured request into an executable agent prompt with clear outcomes, acceptance criteria, and an iterative verification loop. Use when asked to improve a prompt or make a vague task brief execution-ready.
---

# Refine-prompt

Turn the rough request into a standalone, copy-paste prompt for an executing agent. Preserve the user's intent, scope, constraints, and authorization. Return the refined prompt, not advice about writing one.

## Method

1. Extract the actual task, source material, inputs, constraints, audience, and requested deliverables. Keep inferred details distinct from user requirements. If essential material is missing, tell the executing agent to obtain or inspect it before solving; do not invent it.
2. State the task and goal plainly. Describe the observable end state: what must be produced, what each deliverable must contain, its format and location when known, and how the user should be able to use it. Preserve requested depth, style, and simplicity.
3. Turn every requirement into an acceptance criterion with a practical check. The criteria must cover both the working result and the requested final explanation or report.
4. Direct the executing agent to implement the smallest useful increment, run or inspect it, compare the observed result with the criteria, fix gaps, and repeat. Recheck affected criteria after fixes. Continue until all criteria pass or a concrete missing input, permission, or external condition blocks progress.
5. Specify the final response: identify deliverables and how to access or run them, report the checks performed and observed results, and name any unmet criteria or blockers. Never call an unverified result complete.

## Output

Use only the headings needed for clarity, such as **Task**, **Goal and deliverables**, **Acceptance criteria**, **Work loop**, and **Final response**. If asked only to refine, do not execute the underlying task.
