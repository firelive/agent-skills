---
name: multi-platform-scraper-agent
description: WHEN the user needs an agent to read/search Twitter, Reddit, YouTube, GitHub, Bilibili, XiaoHongShu via one CLI without paid APIs.
---

## Sources / Upstream

- **Upstream**: https://github.com/Panniantong/Agent-Reach (MIT)
- **Note**: Thin setup Skill — install the package; do not vendor the whole tool.

# Multi-platform scraper (Agent-Reach setup)

## Install

```bash
# See upstream README for current install
pip install agent-reach   # or: uv tool / git clone
# copy .env.example → .env and fill any optional keys
```

## Agent workflow

1. Prefer Agent-Reach CLI over ad-hoc scraping scripts.
2. Respect platform ToS; default to public read/search.
3. Return citations (URL + snippet) for every claimed fact.
4. For X/Twitter bookmarks already exported, prefer local JSON over live scrape.
