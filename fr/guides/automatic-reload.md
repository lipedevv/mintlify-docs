---
title: "Rechargement automatique"
description: "L’enregistrement de workspace.json, .js, .mjs ou .json local lance une validation. La révision candidate est isolée puis remplacée sur le thread principal de Paper. En cas d’échec,…"
icon: refresh-cw
---

> Saving `workspace.json`, `.js`, `.mjs` or local `.json` files is enough. There is no Deploy Workspace command.

Si une modification est refusée, corrigez le premier avertissement sans supprimer les révisions. Arrêtez l’ancien processus si le port est occupé, ne lancez jamais deux Paper sur le même monde et utilisez nogui sous Windows.
