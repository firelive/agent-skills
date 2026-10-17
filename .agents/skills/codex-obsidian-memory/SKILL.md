---
name: codex-obsidian-memory
description: >-
  When setting up Obsidian as durable memory for a coding agent: folder layout, read/write rules, daily sync, and weekly review.
---

## Sources / Upstream

- **Origin**: authored for firelive/agent-skills from X AI bookmarks catalog
- **License**: free to use in this repo; attribution appreciated
- **Note**: Authored for firelive from X bookmarks catalog.

> This file may be a vendored copy or a thin pointer. Prefer installing/cloning the upstream repo when it ships assets, scripts, or AGPL obligations.

# Codex ↔ Obsidian 永久记忆（安装/约定 Playbook）

把笔记库当作跨项目记忆：偏好、决策习惯、项目细节结构化写入；会话结束强制落盘。

## Goal
Agent 可按需读取；每日同步沟通记录；每周复盘去冗余。

## Setup checklist
1. 选定 Vault 路径；只读先验证，再开写。
2. 约定目录：`Preferences/` `Projects/` `Daily/` `Weekly/` `Decisions/`
3. 模板：
   - Daily：日期、项目、决策、待办、链接
   - Project：目标、现状、关键文件、决策日志
4. 权限：敏感页标记；Agent 默认不外传。
5. 会话协议：开始读相关页 → 结束写回变更（结构化合规段）。
6. 定时：每晚整理当日记录；每周复盘合并冗余。

## Verify
- [ ] Agent 能列出并读取指定文件夹
- [ ] 写回格式符合模板
- [ ] 无密钥写入明文笔记

## Notes
本 Skill 是约定与检查清单；Obsidian/MCP 需在本机另行安装连接。

## Sources
- https://x.com/nini_incrypto_/status/2089738007788335216 (@nini_incrypto_) — 给 Codex 接 Obsidian 作永久记忆

