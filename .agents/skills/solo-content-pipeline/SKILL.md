---
name: solo-content-pipeline
description: >-
  When the user wants a solo creator pipeline: topic → draft → multi-platform publish → metrics feedback, with minimal manual review.
---

## Sources / Upstream

- **Origin**: authored for firelive/agent-skills from X AI bookmarks catalog
- **License**: free to use in this repo; attribution appreciated
- **Note**: Authored for firelive from X bookmarks catalog.

> This file may be a vendored copy or a thin pointer. Prefer installing/cloning the upstream repo when it ships assets, scripts, or AGPL obligations.

# 一人内容流水线

用「薄脚本 + LLM」串起选题→初稿→多平台分发→数据回写；人只审标题与敏感段。

## Inputs
- 内容支柱与禁区
- 平台账号能力（长视频/短视频/图文）
- 可选：历史表现数据

## Outputs
- 周生产计划（1 长 + N 短）
- 自动化步骤清单与人工闸门
- 指标面板字段定义
- 可复用的提示/脚本骨架（概念级，非绑定特定仓库）

## Steps
1. **管道设计**：选题池 → 大纲 → 正文/口播 → 改编（短视频/图文）→ 排期发布 → 数据回写。
2. **人工闸门**：仅标题、敏感声明、品牌红线；其余默认自动。
3. **批量改编规则**：长内容拆 8–12 短；每条独立钩子；统一 CTA。
4. **发布抽象**：按平台写元数据模板（不写死密钥）；失败重试策略。
5. **指标**：曝光、CTR、完播、关注、转化；周更权重（哪类钩子有效）。
6. **参数迭代**：把上周 Top/Bottom 各 3 条结论写回选题提示。

## Architecture notes
- 控制流可用很小的编排脚本（百行级）+ LLM API
- 密钥与账号放环境变量；Skill 里只写步骤与字段

## Checklist
- [ ] 明确人工闸门清单
- [ ] 有数据回写字段
- [ ] 周迭代会议只需看一页面板

## Sources
- https://x.com/qkl2058/status/2053796131143118951 (@qkl2058) — Claude + 130 行 Python 一人内容流水线（月入约 5 万美元）

