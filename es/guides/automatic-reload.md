---
title: "Recarga automática"
description: "Al guardar workspace.json, .js, .mjs o .json local se valida una revisión. La nueva revisión se prepara aislada y se intercambia en el hilo principal de Paper. Si falla, sigue…"
icon: refresh-cw
---

> Saving `workspace.json`, `.js`, `.mjs` or local `.json` files is enough. There is no Deploy Workspace command.

Si se rechaza un cambio, corrige el primer aviso del workspace; no borres revisiones. Si el puerto está ocupado, detén el proceso anterior. Nunca abras dos instancias de Paper sobre el mismo mundo. En Windows usa nogui.
