---
title: "Trikčių šalinimas ir gamybinis sąrašas"
description: "Jei pakeitimas atmestas, taisykite pirmą workspace įspėjimą ir netrinkite revizijų. Sustabdykite seną procesą, jei portas užimtas, neleiskite dviejų Paper tam pačiam pasauliui ir…"
icon: wrench
---

## Production checklist

Prieš gamybą sukurkite workspaces/storage kopijas, patikrinkite start/stop, teises, pilną inventorių ir lėšų trūkumą, saugokite tokeną ir testuokite tiksliai reklamuojamą Paper build.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
