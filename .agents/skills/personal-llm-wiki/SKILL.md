---
name: personal-llm-wiki
description: >-
  When the user wants an incremental personal knowledge wiki built by an LLM (compile-once structured notes), not naive per-query RAG dumping.
---

## Sources / Upstream

- **Origin**: authored for firelive/agent-skills from X AI bookmarks catalog
- **License**: free to use in this repo; attribution appreciated
- **Note**: Authored for firelive from X bookmarks catalog.

> This file may be a vendored copy or a thin pointer. Prefer installing/cloning the upstream repo when it ships assets, scripts, or AGPL obligations.

# 个人 LLM Wiki（增量知识库）

参考开源 LLM Wiki 思路：让模型增量维护结构化 Wiki，知识编译一次并持续更新，而不是每次查询重切全文。

## Inputs
- 原始材料（笔记、PDF、网页、聊天导出）
- 主题边界与隐私红线
- 可选：已有 Wiki 目录

## Outputs
- Wiki 信息架构（主题页/实体页/日志页）
- 切片与更新协议
- 评测问答集 + 每周 Eval 流程
- 引用规范（答必可回溯）

## Steps
1. **架构**：主题索引 → 概念页 → 来源页 → 日记/变更日志。
2. **切片策略**：按语义单元，不按固定 token 盲切；保留标题路径。
3. **编译**：材料 → 结构化页（定义、要点、链接、未决问题）；只增量补丁。
4. **检索**：先 Wiki 内链，再回源；强制引用。
5. **重排与拒答**：低置信则说不知道并建议补材料。
6. **Eval**：固定 20 问业务集，每周跑，盯正确率与引用率。

## Anti-patterns
- 只堆 Embedding 不维护结构化页
- 无引用的自信胡答
- 把隐私材料送进不可控第三方（先本地策略）

## Checklist
- [ ] 有信息架构草图
- [ ] 有更新协议（何时重编译）
- [ ] 有 Eval 集

## Sources
- https://x.com/Jolyne_AI/status/2071171770976223441 (@Jolyne_AI) — 开源 LLM Wiki：增量个人知识库

