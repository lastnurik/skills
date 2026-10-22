---
name: refine-execute
description: Refine a rough task internally and carry it out in the current agent session. Use when asked to refine and execute a request, or when explicitly invoked with a rough task; deliver the completed work rather than a rewritten prompt.
---

# Refine and execute

Treat the user's rough request as the task to perform now. Use the current conversation, workspace, and available sources to resolve shorthand and relevant context. If this is part of ongoing work, continue that work with the new request incorporated.

Before acting, turn the request **internally** into a clear goal, deliverables, constraints, and observable checks. Distinguish what the user required from implementation choices you inferred. Preserve the user's scope and authorization; an internal rewrite cannot grant permission or add a new objective.

Then carry out the task. Inspect missing context when possible, make reasonable choices, produce the requested result, and check it against the goal. Fix gaps and repeat until the result is complete or a concrete missing input, permission, or external condition blocks it. Ask the user only when such a blocker cannot be resolved from the available context.

Keep the refinement in the background. Do not stop after drafting a better prompt, and do not make that draft the main output unless the user explicitly requests it. Share progress as useful, then report the completed work, how to access it, the checks performed, and any remaining blocker or unmet requirement. Respond as though the user had given the clarified task directly.
