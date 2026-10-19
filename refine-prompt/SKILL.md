---
name: refine-prompt
description: Refine an unstructured request into an executable agent prompt with clear outcomes, acceptance criteria, and an iterative verification loop. Use when asked to improve a prompt or make a vague task brief execution-ready.
---

# Refine-prompt

Produce a copy-paste prompt that an agent can execute and verify. Preserve the user's intent, scope, constraints, and authorization.

## Method

1. Extract the required task, deliverables, constraints, inputs, and audience from the request and available references. Keep proposed details distinct from requirements. If essential source material is missing, instruct the executing agent to obtain or inspect it; do not invent it.
2. State the desired end result and acceptance criteria that can be checked against the source request. Give each criterion a practical verification method. Keep the solution's expected complexity proportional to the task.
3. Instruct the executing agent to implement the smallest useful increment, run or inspect it, compare the observed result with the criteria, fix gaps, and repeat. Recheck affected criteria after each fix. Continue until all criteria pass or a specific missing input, permission, or external condition prevents progress.
4. Require a final report with deliverables, verification performed and observed results, and any unmet criteria or blockers. Never describe an unverified result as complete.

## Output

Write direct instructions to the executing agent. Use only the headings needed to make the prompt clear. If the user asks only for refinement, deliver the prompt without executing the underlying task.
