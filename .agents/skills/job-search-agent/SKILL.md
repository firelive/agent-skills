---
name: job-search-agent
description: WHEN the user wants BOSS直聘/job search via local CLI, shortlist filtering, or a job-hunt agent workflow.
---

## Sources / Upstream

- **Upstream CLI**: https://github.com/can4hou6joeng4/boss-agent-cli (MIT)
- **Also starred**: MadsLorentzen/ai-job-search, career-ops-hq/career-ops, interviewstreet/hiring-agent
- **Note**: This is a thin wrapper Skill. Do not reinvent the CLI; install and drive it.

# Job Search Agent (wrapper)

## Install

```bash
# Prefer uv / pip from upstream README
git clone https://github.com/can4hou6joeng4/boss-agent-cli.git
cd boss-agent-cli
# follow README: uv sync / pip install -e .
```

## How to use with an agent

1. Confirm the user wants **local-assist** BOSS Zhipin search (compliant, low-risk defaults).
2. Run the CLI for search → welfare filter → shortlist → JSON envelope output.
3. Summarize shortlist in Chinese; never auto-apply without explicit user approval.
4. Pair with `interview-hr-simulator` for mock interviews on shortlisted roles.

## Takeaways from firelive X bookmarks catalog

- Prefer structured JSON envelopes so Moi/Codex can parse results.
- Keep human-in-the-loop for apply / message / phone steps.
- Combine with resume/storybank skills rather than one mega-agent.
