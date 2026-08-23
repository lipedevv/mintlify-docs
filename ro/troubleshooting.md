---
title: "Depanare și listă pentru producție"
description: "Dacă o schimbare este respinsă, repară primul avertisment fără a șterge revizii. Oprește procesul vechi dacă portul e ocupat, nu rula două Paper pe aceeași lume și folosește nogui…"
icon: wrench
---

## Production checklist

Înainte de producție: salvează workspaces/storage, testează pornire/oprire, permisiuni, inventar plin și fonduri insuficiente, protejează tokenul și testează exact buildul Paper anunțat.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
