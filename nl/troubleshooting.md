---
title: "Probleemoplossing en productiechecklist"
description: "Bij een afgewezen wijziging los je de eerste workspace-waarschuwing op zonder revisies te wissen. Stop het oude proces bij een bezette poort, start nooit twee Paper-instanties voor…"
icon: wrench
---

## Production checklist

Voor productie: maak backups, test start/stop, rechten, volle inventaris en onvoldoende saldo, bescherm het token en test exact de geadverteerde Paper-build.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
