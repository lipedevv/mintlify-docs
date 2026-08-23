---
title: "Dépannage et contrôle de production"
description: "Si une modification est refusée, corrigez le premier avertissement sans supprimer les révisions. Arrêtez l’ancien processus si le port est occupé, ne lancez jamais deux Paper sur…"
icon: wrench
---

## Production checklist

Avant production : sauvegardez workspaces et storage, testez démarrage/arrêt, droits, inventaire plein et solde insuffisant, protégez le jeton et testez exactement le build Paper annoncé.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
