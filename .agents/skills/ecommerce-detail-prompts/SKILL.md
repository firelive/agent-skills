---
name: ecommerce-detail-prompts
description: >-
  When the user needs an ecommerce detail-page pipeline: product image → selling points → full set of detail/KV image prompts for designers or image models.
---

## Sources / Upstream

- **Origin**: authored for firelive/agent-skills from X AI bookmarks catalog
- **License**: free to use in this repo; attribution appreciated
- **Note**: Authored for firelive from X bookmarks catalog.

> This file may be a vendored copy or a thin pointer. Prefer installing/cloning the upstream repo when it ships assets, scripts, or AGPL obligations.

# 电商详情页全套提示词流程

固定链：产品图 → 卖点与视觉重点 → 全套详情分镜提示词（可直接给设计师或文生图）。

## Inputs
- 产品图（或产品名+规格）
- 品牌约束：主色/字体/禁用词/竞品规避
- 平台（淘宝/抖音/独立站等）与类目

## Outputs
- 卖点清单（功能/情感/信任）
- 10 张级详情分镜表（用途、文案点、构图、标注）
- 每张图的完整提示词
- SKU 批量时的表格驱动模板

## Steps
1. **读图提炼**：材质、结构、使用场景、差异点；标视觉焦点。
2. **卖点排序**：痛点→利益→证据（参数/认证/对比）。
3. **分镜框架**（可按类目裁剪）：
   - 主 KV / 场景种草 / 痛点击穿 / 卖点拆解 ×N / 规格参数 / 对比 / 社会责任或售后 / 促销收束
4. **提示词生成**：统一风格锁（色板、镜头、留白、字体气质）；每张含：主体、场景、文字占位、禁止项。
5. **设计师标注**：安全区、字号层级、必出信息。
6. **批量**：SKU 表列驱动（颜色/规格替换），主结构不变。

## Checklist
- [ ] 品牌色与禁用词已写入每条提示
- [ ] 分镜覆盖种草→信任→转化
- [ ] 输出可复制给设计或模型

## Sources
- https://x.com/yyyole/status/2002018915610943628 (@yyyole) — 产品图 → 卖点 → 全套电商详情页提示词流程

