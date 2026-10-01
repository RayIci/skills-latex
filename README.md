# skills-latex

Agent skills for writing LaTeX, installable with [skills.sh](https://skills.sh).

## Install

```bash
npx skills add RayIci/skills-latex
```

List the available skills without installing:

```bash
npx skills add RayIci/skills-latex --list
```

Install a single skill:

```bash
npx skills add RayIci/skills-latex --skill writing-latex
```

## Skills

| Skill | Description |
|-------|-------------|
| [`writing-latex`](skills/writing-latex/SKILL.md) | Write, restructure and debug LaTeX documents: multi-file structure, a shared preamble of coloured explanation boxes, step-by-step math, TikZ/pgfplots figures, and a compile-and-look verification loop. |

## Adding a skill

Each skill is a folder under `skills/` with a `SKILL.md` file that starts with YAML frontmatter:

```markdown
---
name: my-skill          # lowercase, hyphens allowed; must be unique
description: What the skill does and when the agent should use it.
---
```

Supporting files (`references/`, `assets/`, `scripts/`) go next to `SKILL.md`. Run `npx skills add . --list` from the repo root to check that the CLI finds the new skill.
