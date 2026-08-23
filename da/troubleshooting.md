---
title: "Fejlfinding og produktionscheckliste"
description: "Hvis en ændring afvises, ret den første workspace-advarsel uden at slette revisioner. Stop gammel proces ved optaget port, kør aldrig to Paper på samme world og brug nogui i…"
icon: wrench
---

## Production checklist

Før produktion: sikkerhedskopiér workspaces/storage, test start/stop, rettigheder, fuldt inventory og utilstrækkelig saldo, beskyt token og test præcis den annoncerede Paper-build.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
