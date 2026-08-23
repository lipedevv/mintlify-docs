---
title: "Riešenie problémov a produkčný zoznam"
description: "Pri odmietnutej zmene opravte prvé varovanie a nemažte revízie. Zastavte starý proces pri obsadenom porte, nespúšťajte dva Paper nad rovnakým svetom a vo Windows používajte nogui."
icon: wrench
---

## Production checklist

Pred produkciou zálohujte workspaces/storage, otestujte štart/stop, oprávnenia, plný inventár a nedostatok peňazí, chráňte token a testujte presne propagovaný Paper build.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
