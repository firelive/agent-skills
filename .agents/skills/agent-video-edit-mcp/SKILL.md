---
name: agent-video-edit-mcp
description: WHEN the user wants MCP/agent-driven video editing entrypoints backed by OpenMontage rather than a greenfield MCP.
---

## Sources / Upstream

- **Upstream**: https://github.com/calesthio/OpenMontage (AGPL-3.0)
- **Related catalog id**: `video-production-skills`

# Agent video edit MCP (OpenMontage entry)

1. Clone OpenMontage; read `AGENT_GUIDE.md` / MCP-related docs in-repo.
2. Expose only the edit/export tools the user needs (trim, captions, assemble).
3. Keep media paths local; never upload private footage without explicit approval.
4. AGPL notice applies to network services using modified code.
