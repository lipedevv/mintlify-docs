---
title: "Workspace-Struktur"
description: "Ordnername und Manifest-id müssen übereinstimmen. Der Einstieg muss .js oder .mjs sein. Relative JavaScript-/JSON-Importe bleiben im Workspace; versteckte Ordner, nodemodules, dist…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Erstes Skript

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
