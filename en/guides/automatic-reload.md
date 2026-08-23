---
title: "Automatic reload"
description: "Saving workspace.json, .js, .mjs or local .json files triggers a debounced validation. A candidate revision is prepared in isolation and swapped on the Paper main thread. If it…"
icon: refresh-cw
---

> Saving `workspace.json`, `.js`, `.mjs` or local `.json` files is enough. There is no Deploy Workspace command.

If a saved change is rejected, read the first workspace warning and fix the source; do not delete revisions. If the port is busy, stop the old server process. If the world is locked, never start a second Paper instance. Use nogui on Windows to avoid an AWT shutdown hang.
