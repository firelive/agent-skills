---
name: chrome-devtools-mcp
description: >-
  When installing Chrome DevTools MCP for browser automation: enable debugging, lock a read-only first path, then script open→click→screenshot→assert.
---

## Sources / Upstream

- **Origin**: authored for firelive/agent-skills from X AI bookmarks catalog
- **License**: free to use in this repo; attribution appreciated
- **Note**: Authored for firelive from X bookmarks catalog.

> This file may be a vendored copy or a thin pointer. Prefer installing/cloning the upstream repo when it ships assets, scripts, or AGPL obligations.

# Chrome DevTools MCP 安装与验收

用官方 DevTools MCP 做浏览器自动化：配置简单，能力强于普通 browser MCP。

## Setup checklist
1. 按 Google/Chrome DevTools MCP 文档一键接入对应编程工具。
2. 授权本机浏览器调试端口；确认仅本地。
3. **先只读模式**：打开页面、截图、断言文本；敏感站不填表。
4. 固化回归脚本：打开→点选→截图→断言。
5. 再按需放开表单填写（另开权限闸门）。

## Verify
- [ ] 工具可启动/附着浏览器
- [ ] 截图与 DOM 断言成功
- [ ] 敏感站点策略已文档化

## Safety
- 不要自动化银行/支付除非用户明确要求并本地确认
- 本 Skill 是安装清单，不默认已连接

## Sources
- https://x.com/yaohui12138/status/1980841732830085553 (@yaohui12138) — Chrome DevTools MCP 接管浏览器自动化

