---
title: "Felsökning och produktionschecklista"
description: "Om en ändring avvisas, rätta första workspace-varningen utan att radera revisioner. Stoppa gammal process vid upptagen port, kör inte två Paper mot samma värld och använd nogui i…"
icon: wrench
---

## Production checklist

Före produktion: säkerhetskopiera workspaces/storage, testa start/stopp, behörigheter, fullt inventory och otillräckligt saldo, skydda token och testa exakt annonserad Paper-build.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
