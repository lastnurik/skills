---
name: refine-prompt
description: Turn a rough request into a clear prompt that defines the goal, deliverables, and an execute-verify loop. Return only that prompt, with no progress messages; never perform the task.
---

# Refine prompt

Rewrite the user's request as a standalone prompt for another agent. Define the goal the user wants, the deliverables that would meet it, and how to tell whether they work. Preserve the user's scope and constraints without inventing requirements.

Instruct the agent to execute the task, verify the result against the goal, fix any gaps, and repeat until the goal is met or a specific blocker prevents further progress.

Return only the refined prompt, with no progress messages or commentary. Never carry out the underlying task, even if the request asks you to.
