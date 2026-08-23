---
title: "Solução de problemas e checklist de produção"
description: "Se uma alteração for rejeitada, corrija o primeiro aviso do workspace e não apague revisões. Encerre o processo antigo se a porta estiver ocupada, nunca rode dois Paper no mesmo…"
icon: wrench
---

## Production checklist

Antes da produção: faça backup de workspaces e storage, teste início/parada/reinício, permissões, inventário cheio e saldo insuficiente, proteja o token e valide exatamente a build do Paper anunciada.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
