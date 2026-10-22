# Skills

This repository contains the following agent skill:

| Skill | What it does |
| --- | --- |
| [`refine-prompt`](refine-prompt/SKILL.md) | Returns a prompt defining the user's goal, deliverables, and an execute-verify loop. |
| [`refine-execute`](refine-execute/SKILL.md) | Uses the same refinement internally, then executes and verifies the task. |

## Install

Use the [Skills CLI](https://github.com/vercel-labs/skills) to install from this GitHub repository:

```bash
npx skills add lastnurik/skills
```

To list the available skills without installing them:

```bash
npx skills add lastnurik/skills --list
```

To install one skill:

```bash
npx skills add lastnurik/skills --skill refine-prompt
npx skills add lastnurik/skills --skill refine-execute
```

`refine-prompt` returns a rewritten prompt. `refine-execute` carries out the request and reports the result.

The CLI discovers each skill from its top-level `SKILL.md` folder. No npm package or build step is required.
