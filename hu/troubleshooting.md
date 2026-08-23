---
title: "Hibaelhárítás és élesítési ellenőrzés"
description: "Elutasított mentésnél javítsd az első workspace figyelmeztetést, ne töröld a revíziókat. Foglalt portnál állítsd le a régi folyamatot, ne futtass két Papert ugyanazon a világon,…"
icon: wrench
---

## Production checklist

Élesítés előtt mentsd a workspaces/storage adatokat, teszteld a start/stop, jogosultság, tele leltár és kevés egyenleg esetét, védd a tokent és pontosan a hirdetett Paper buildet teszteld.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
