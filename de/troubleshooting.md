---
title: "Fehlerbehebung und Produktionscheckliste"
description: "Bei abgelehnten Änderungen die erste Workspace-Warnung beheben; Revisionen nicht löschen. Alte Prozesse bei belegtem Port stoppen, nie zwei Paper-Instanzen auf derselben Welt…"
icon: wrench
---

## Production checklist

Vor Produktion Workspaces und Storage sichern, Start/Stopp/Neustart, Rechte, volles Inventar und zu wenig Guthaben prüfen, Token schützen und exakt den beworbenen Paper-Build testen.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
