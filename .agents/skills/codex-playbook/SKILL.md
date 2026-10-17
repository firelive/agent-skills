---
name: codex-playbook
description: WHEN setting up Codex with shared skills from mattpocock/skills, awesome-claude-skills, and firelive/agent-skills.
---

## Sources / Upstream

- https://github.com/mattpocock/skills
- https://github.com/ComposioHQ/awesome-claude-skills
- This repo: https://github.com/firelive/agent-skills (`.agents/skills/`)

# Codex playbook (shared skills)

## Layout Codex expects

Put or symlink skills under `.agents/skills/<id>/SKILL.md` (this repo already uses that layout).

## Recommended order

1. Clone this repo or sparse-checkout `.agents/skills/`.
2. Add mattpocock engineering skills you actually use (tdd, pr, code-review).
3. Add domain skills from awesome-claude-skills sparingly.
4. Keep secrets out of skill files; use env / MCP auth.

## Do not

- Vendor entire OpenMontage or huge monorepos into Codex skills.
- Mix AGPL and proprietary product code without legal review.
