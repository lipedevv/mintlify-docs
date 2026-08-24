---
name: nexora-development
description: Build, review, and debug JavaScript workspaces for Nexora on Paper servers. Use for commands, events, GUIs, shops, persistence, HTTP, scheduling, security, and runtime troubleshooting implemented through the documented Nexora API.
license: Proprietary documentation; Nexora software may not be resold or redistributed
compatibility: Nexora 1.0.0; Paper 1.20.6 through 26.2; Java 21 for Paper 1.20.6–1.21.11 and Java 25 for Paper 26.x
metadata:
  author: lipedevv
  version: "1.0.0"
---

# Nexora development

Create production-ready Nexora workspaces using only the public JavaScript API documented at `https://nexora.mintlify.site/en/reference/javascript-api`.

## Core invariants

- Write JavaScript in `.js` or `.mjs` files. Do not introduce TypeScript, Node.js dependencies, bundlers, build output, or manual deployment.
- Place a workspace in `plugins/NexoraEngine/workspaces/<workspace-id>`. The directory name and `workspace.json` id must match.
- Saving supported workspace files triggers automatic validation and reload. Preserve the previously running revision when validation fails.
- Prefer Safe Mode. Use Native Mode only for an explicit Paper/Bukkit requirement and declare the exact native capability.
- Never invent API methods, event names, manifest fields, or capabilities. Consult `/llms.txt` and the API reference when uncertain.
- Keep callbacks bounded. Use the scheduler for delayed or repeated work and the asynchronous database/HTTP surfaces for I/O.

## Workflow

1. Read `https://nexora.mintlify.site/llms.txt` and open the relevant Markdown reference pages.
2. Define the workspace id, capabilities, configuration, persistence model, commands, events, and GUI behavior.
3. Create `workspace.json`, `index.js`, and only the service modules actually needed.
4. Validate permissions, player-only requirements, null/offline players, inventory capacity, transaction outcomes, and reload cleanup.
5. Explain exact in-game commands and edge cases for testing on Paper.

## Security and correctness

- Treat all command arguments, configuration values, database rows, and HTTP responses as untrusted input.
- Use parameterized SQL. Use database transactions for related writes and enforce affected-row expectations.
- For purchases, debit only when funds are sufficient; deliver only when inventory capacity is confirmed; compensate or refund if delivery fails.
- Cancel tasks, listeners, resources, and pending work during workspace shutdown or reload.
- Do not expose secrets in source files, logs, GUI lore, or messages.

## References

- Index: `https://nexora.mintlify.site/llms.txt`
- Complete context: `https://nexora.mintlify.site/llms-full.txt`
- Workspace manifest: `https://nexora.mintlify.site/en/reference/manifest.md`
- JavaScript API: `https://nexora.mintlify.site/en/reference/javascript-api.md`
- Configuration: `https://nexora.mintlify.site/en/reference/configuration.md`
- Troubleshooting: `https://nexora.mintlify.site/en/troubleshooting.md`
