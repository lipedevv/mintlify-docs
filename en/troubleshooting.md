---
title: "Troubleshooting and production checklist"
description: "If a saved change is rejected, read the first workspace warning and fix the source; do not delete revisions. If the port is busy, stop the old server process. If the world is…"
icon: wrench
---

## Production checklist

Before production: back up workspaces and storage, test start/stop/restart, verify permissions as player and console, test full inventories and insufficient funds, keep Native Mode off, retain the admin token securely, and test the exact Paper build you advertise.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
