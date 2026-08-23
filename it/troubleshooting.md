---
title: "Risoluzione problemi e checklist di produzione"
description: "Se una modifica è rifiutata, correggi il primo avviso senza eliminare revisioni. Ferma il vecchio processo se la porta è occupata, non avviare due Paper sullo stesso mondo e usa…"
icon: wrench
---

## Production checklist

Prima della produzione esegui backup di workspaces/storage, prova avvio/arresto, permessi, inventario pieno e saldo insufficiente, proteggi il token e testa esattamente la build Paper dichiarata.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
