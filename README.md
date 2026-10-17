# firelive/agent-skills

Shared **Agent Skills** for Moi / Codex / Claude Code.

中文：这个仓库把我在 GitHub 上 star 过的优质 Skill 做成可安装索引，并补齐收藏清单里暂时没有上游的自定义 Skill。优先用上游，不重复造轮子。

English: Index of starred upstream Agent Skills plus custom fillers. Layout: `.agents/skills/<id>/SKILL.md`.

## Install

```bash
git clone https://github.com/firelive/agent-skills.git
# Symlink or copy .agents/skills/* into your agent skills directory
```

Codex / many agents auto-load `.agents/skills/*/SKILL.md`.

## Catalog (25)

| id | mode | preferred upstream |
|----|------|-------------------|
| `book-to-skill-distill` | vendored | `kangarooking/cangjie-skill` |
| `de-ai-flavor-writing` | vendored | `op7418/Humanizer-zh` |
| `anti-sycophancy-prompts` | authored | (authored) |
| `job-search-agent` | pointer | `can4hou6joeng4/boss-agent-cli` |
| `design-taste-skills` | vendored | `alchaincyf/huashu-design` |
| `personal-llm-wiki` | authored | (authored) |
| `creator-media-skills` | authored | (authored) |
| `ppt-skills-ranker` | vendored | `op7418/guizang-ppt-skill` |
| `codex-obsidian-memory` | authored | (authored) |
| `video-production-skills` | pointer | `calesthio/OpenMontage` |
| `agent-video-edit-mcp` | pointer | `calesthio/OpenMontage` |
| `multi-platform-scraper-agent` | pointer | `Panniantong/Agent-Reach` |
| `pixel-rag-browser` | authored | (authored) |
| `chrome-devtools-mcp` | authored | (authored) |
| `handdrawn-story-skill` | vendored | `threerocks/hand-drawn-styles` |
| `claude-code-onboarding` | pointer | `mattpocock/skills` |
| `codex-playbook` | pointer | `mattpocock/skills` |
| `digital-human-pipeline` | authored | (authored) |
| `china-grassroots-logic-skill` | vendored | `ayi-ai/nie-grassroots-logic` |
| `ai-pm-job-guide` | authored | (authored) |
| `youtube-content-workflow` | authored | (authored) |
| `sales-script-coach` | authored | (authored) |
| `solo-content-pipeline` | authored | (authored) |
| `interview-hr-simulator` | vendored | `noamseg/interview-coach-skill` |
| `ecommerce-detail-prompts` | authored | (authored) |

## Strong upstream matches

| Our id | Upstream | License |
|--------|----------|---------|
| china-grassroots-logic-skill | [ayi-ai/nie-grassroots-logic](https://github.com/ayi-ai/nie-grassroots-logic) | MIT |
| book-to-skill-distill | [kangarooking/cangjie-skill](https://github.com/kangarooking/cangjie-skill) | MIT |
| de-ai-flavor-writing | [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) (+ [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop)) | MIT |
| handdrawn-story-skill | [threerocks/hand-drawn-styles](https://github.com/threerocks/hand-drawn-styles) | MIT |
| ppt-skills-ranker | [op7418/guizang-ppt-skill](https://github.com/op7418/guizang-ppt-skill) (also [chuspeeism/dashi-ppt-skill](https://github.com/chuspeeism/dashi-ppt-skill)) | AGPL-3.0 |
| design-taste-skills | [alchaincyf/huashu-design](https://github.com/alchaincyf/huashu-design) | MIT |
| interview-hr-simulator | [noamseg/interview-coach-skill](https://github.com/noamseg/interview-coach-skill) | MIT |

## Pointer / setup skills (do not vendor whole repos)

| Our id | Upstream |
|--------|----------|
| job-search-agent | [can4hou6joeng4/boss-agent-cli](https://github.com/can4hou6joeng4/boss-agent-cli) |
| multi-platform-scraper-agent | [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) |
| video-production-skills | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) |
| agent-video-edit-mcp | same OpenMontage |
| claude-code-onboarding | [mattpocock/skills](https://github.com/mattpocock/skills) + [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) |
| codex-playbook | same indexes |

## Authored gaps (no clear starred SKILL.md match)

`ecommerce-detail-prompts`, `sales-script-coach`, `youtube-content-workflow`, `solo-content-pipeline`, `ai-pm-job-guide`, `anti-sycophancy-prompts`, `creator-media-skills`, `personal-llm-wiki`, `codex-obsidian-memory`, `pixel-rag-browser`, `chrome-devtools-mcp`, `digital-human-pipeline`

## License

- Vendored MIT skills: see each folder's `UPSTREAM_LICENSE` and `licenses/`.
- Vendored AGPL (`guizang-ppt-skill`): see `licenses/op7418_guizang-ppt-skill.LICENSE` — comply if you modify and provide network services.
- Pointer skills: follow upstream licenses; we only document install steps.
- Authored skills in this repo: free to use with the repo; attribution appreciated.

## Sync policy

Prefer updating from upstream `SKILL.md` over rewriting. Custom authored skills stay until a better starred match appears.
