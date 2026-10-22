# Skills

This repository contains the following agent skill:

| Skill | What it does |
| --- | --- |
| [`refine-prompt`](refine-prompt/SKILL.md) | Turns a rough request into an executable agent prompt with clear outcomes, acceptance criteria, and a verification loop. |
| [`refine-execute`](refine-execute/SKILL.md) | Clarifies a rough request internally, then completes the task in the current agent session. |

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
