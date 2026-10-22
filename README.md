# Skills

This repository contains the following agent skill:

| Skill | What it does |
| --- | --- |
| [`refine-prompt`](refine-prompt/SKILL.md) | Turns a rough request into an executable agent prompt with clear outcomes, acceptance criteria, and a verification loop. |

## Install

Use the [Skills CLI](https://github.com/vercel-labs/skills) to install from this GitHub repository:

```bash
npx skills add lastnurik/skills
```

To list the available skills without installing them:

```bash
npx skills add lastnurik/skills --list
```

To install only `refine-prompt`:

```bash
npx skills add lastnurik/skills --skill refine-prompt
```

The CLI discovers `refine-prompt/SKILL.md` directly from this repository. No npm package or build step is required.
