---
title: "Řešení problémů a produkční kontrola"
description: "Při odmítnutí změny opravte první varování a nemažte revize. Uvolněte obsazený port, nespouštějte dva Paper nad stejným světem a ve Windows používejte nogui."
icon: wrench
---

## Production checklist

Před produkcí zálohujte workspaces/storage, otestujte start/stop, oprávnění, plný inventář a nedostatek peněz, chraňte token a ověřte přesný inzerovaný Paper build.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
