---
title: "Rozwiązywanie problemów i lista produkcyjna"
description: "Po odrzuceniu zmiany popraw pierwszy komunikat workspace, bez kasowania rewizji. Zatrzymaj stary proces przy zajętym porcie, nie uruchamiaj dwóch Paper dla jednego świata i używaj…"
icon: wrench
---

## Production checklist

Przed produkcją wykonaj kopie workspaces/storage, sprawdź start/stop, uprawnienia, pełny ekwipunek i brak środków, chroń token i testuj dokładnie reklamowany build Paper.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
