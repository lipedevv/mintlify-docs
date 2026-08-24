---
name: nexora-workspace
description: Create or modify safe, automatically reloaded JavaScript workspaces for Nexora, including manifests, commands, events, scheduling, storage, databases, and HTTP.
license: Proprietary documentation
metadata:
  author: lipedevv
  version: "1.0.0"
---

# Nexora workspace development

Use this skill when implementing ordinary Nexora workspace behavior outside a specialized transactional GUI flow.

- Read the manifest and JavaScript API references through `https://nexora.mintlify.site/llms.txt` before choosing symbols.
- Use `.js` or `.mjs`; do not add TypeScript, Node.js packages, bundling, build directories, or deploy commands.
- Match the workspace directory name to `workspace.json` `id` and declare only the capabilities the implementation actually uses.
- Prefer Safe Mode. Native Mode is an explicit trust decision, not a workaround for an undocumented API.
- Register commands, events, and scheduled tasks during startup and release their resources on shutdown/reload.
- Validate player availability, permissions, optional arguments, configuration types, database results, HTTP status, and timeouts.
- Provide a test checklist covering startup, successful paths, rejected inputs, reload, shutdown, and persistence after restart.

If a requested symbol is not documented, report it as unsupported and propose a documented design instead of inventing an API.
