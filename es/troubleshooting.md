---
title: "Solución de problemas y lista de producción"
description: "Si se rechaza un cambio, corrige el primer aviso del workspace; no borres revisiones. Si el puerto está ocupado, detén el proceso anterior. Nunca abras dos instancias de Paper…"
icon: wrench
---

## Production checklist

Antes de producción: crea copias de workspaces y storage, prueba inicio y apagado, permisos, inventario lleno y saldo insuficiente, protege el token y valida exactamente la compilación de Paper anunciada.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
