---
name: digital-human-pipeline
description: >-
  When building a digital-human avatar pipeline via APIs: voice, script rewrite, talking-head video—setup steps and verification, including packaging for reuse.
---

## Sources / Upstream

- **Origin**: authored for firelive/agent-skills from X AI bookmarks catalog
- **License**: free to use in this repo; attribution appreciated
- **Note**: Authored for firelive from X bookmarks catalog.

> This file may be a vendored copy or a thin pointer. Prefer installing/cloning the upstream repo when it ships assets, scripts, or AGPL obligations.

# 数字人形象六步流程（API 封装）

步骤均可 API 化：形象 → 语音 → 口播稿 → 改写 → 口播视频 → 文案获取/复用。

## Pipeline
1. 形象生成/选定（形象 ID）
2. 音色/语音合成
3. 口播稿生成
4. 稿件改写（平台语气）
5. 驱动口播视频
6. 导出与文案归档

## Setup checklist
1. 准备各步 API 密钥与配额告警。
2. 先跑通最小闭环（10s 样片）。
3. 封装为本地小工具或 Agent Skill（输入主题→出口播成片路径）。
4. 质量闸门：口型、错别字、违禁词。

## Verify
- [ ] 六步都有成功日志
- [ ] 样片可发布级（或明确差距）
- [ ] 密钥不入库

## Note
作者反馈「原流程不好用故封装软件」——优先可复现封装，而不是散落手工点击。

## Sources
- https://x.com/xiaomovps/status/2074432448335851688 (@xiaomovps) — Codex 生成数字人形象的六步流程与封装

