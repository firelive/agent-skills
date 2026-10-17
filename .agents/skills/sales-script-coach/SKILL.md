---
name: sales-script-coach
description: >-
  When the user wants to improve sales scripts, handle objections, or generate talk tracks from customer persona and high-converting examples.
---

## Sources / Upstream

- **Origin**: authored for firelive/agent-skills from X AI bookmarks catalog
- **License**: free to use in this repo; attribution appreciated
- **Note**: Authored for firelive from X bookmarks catalog.

> This file may be a vendored copy or a thin pointer. Prefer installing/cloning the upstream repo when it ships assets, scripts, or AGPL obligations.

# 销冠话术教练

输入客户画像与异议，输出可试用的话术卡；用高转化样本做 few-shot，并支持 A/B。

## Inputs
- 产品/报价与边界（不能承诺什么）
- 客户画像（角色、痛点、决策链、预算信号）
- 可选：历史高转化话术样本、失败通话要点

## Outputs
- 话术卡：开场 / 探需 / 价值主张 / 异议处理 / 逼单 / 跟进
- 按异议类型的改写表（价格、信任、竞品、时机、权限）
- A/B 两版 + 选用建议
- 通话后复盘模板

## Steps
1. **校准样本**：若有高转化话术，提炼结构（不是背原文）：开场模式、问题序列、证据类型。
2. **探需问题**：先问现状与代价，再谈方案；禁止一上来讲功能清单。
3. **价值映射**：痛点 → 结果指标 → 证据（案例/数据/演示）。
4. **异议库**：对每类异议给「认同→澄清→证据→二选一推进」。
5. **A/B**：版 A 更直接，版 B 更顾问式；标明适用客户类型。
6. **红线**：不虚构案例/折扣权限；不确定就标明需确认。
7. **落地**：输出一页话术卡，可直接贴进 CRM/笔记。

## Checklist
- [ ] 每条异议有完整四步回应
- [ ] 有明确下一步（约会/演示/报价）
- [ ] 无无法兑现的承诺

## Sources
- https://x.com/imwsl90/status/2079846369356026244 (@imwsl90) — 销冠助手：用 Claude 改进话术辅助成交

