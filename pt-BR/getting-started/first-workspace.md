---
title: "Estrutura do workspace"
description: "O nome da pasta deve ser igual ao id do manifesto. A entrada precisa terminar em .js ou .mjs. Imports JavaScript/JSON relativos ficam dentro do workspace; pastas ocultas,…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Primeiro script

```js
on("playerJoin", ({ player }) => {
  player.send("<green>Welcome to Nexora!</green>");
});

command("heal", {
  permission: "example.heal",
  playerOnly: true,
  execute({ player }) {
    player.heal();
    player.send("<green>Healed.</green>");
  }
});
```
