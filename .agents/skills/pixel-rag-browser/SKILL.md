---
name: pixel-rag-browser
description: >-
  When setting up screenshot/vision-based page reading (PixelRAG-style) instead of brittle HTML scraping—install, verify, and know when to use it.
---

## Sources / Upstream

- **Origin**: authored for firelive/agent-skills from X AI bookmarks catalog
- **License**: free to use in this repo; attribution appreciated
- **Note**: Authored for firelive from X bookmarks catalog.

> This file may be a vendored copy or a thin pointer. Prefer installing/cloning the upstream repo when it ships assets, scripts, or AGPL obligations.

# PixelRAG / 像素级读网页 Playbook

跳过脆弱 HTML 解析：截图 → 视觉模型读答案；适合强渲染/反爬页面。

## When to use
- DOM 抓取失败或内容在画布/图片中
- 需要「看到」布局与图表

## Setup checklist
1. 按开源项目安装（含 Claude Code/Codex 插件若提供）。
2. 配置浏览器截图依赖与视觉模型密钥。
3. 隐私：脱敏后再送视觉模型。

## Verify
- [ ] 对静态文档页能抽出指定字段
- [ ] 对图表页能回答数值问题
- [ ] 记录成本（截图+视觉 token）

## Fallback
DOM/文本 RAG 仍优先用于纯文本站点。

## Sources
- https://x.com/LTChives/status/2068935453525606661 (@LTChives) — PixelRAG：截图像素级读网页

