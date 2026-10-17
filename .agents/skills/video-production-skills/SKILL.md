---
name: video-production-skills
description: WHEN the user wants an agentic video production studio (pipelines, tools, skills) via OpenMontage rather than inventing a new stack.
---

## Sources / Upstream

- **Upstream**: https://github.com/calesthio/OpenMontage (AGPL-3.0)
- **Note**: Large monorepo (700+ skill files). This Skill only tells you how to set it up — do not dump the tree into `.agents/skills/`.

# Video production skills (OpenMontage setup)

## Install / wire-up

```bash
git clone https://github.com/calesthio/OpenMontage.git
cd OpenMontage
# Follow README / AGENTS.md / CODEX.md / CURSOR.md for your agent host
```

## Agent rules

1. Use OpenMontage's own skill files in-repo; symlink or point your agent docs at them.
2. AGPL-3.0: if you ship a network service using modified OpenMontage, publish corresponding source.
3. Prefer one pipeline at a time (script → storyboard → edit → export).
