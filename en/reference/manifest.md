---
title: "Workspace manifest"
description: "Only id, name and version are mandatory; entry defaults to index.js. Declare every capability used by the script. Native Mode requires both server-wide enablement and workspace…"
icon: blocks
---

```json
{
  "id": "my-workspace",
  "name": "My Workspace",
  "version": "1.0.0",
  "entry": "index.js",
  "permissions": [
    "minecraft.players",
    "minecraft.commands",
    "minecraft.inventory",
    "database",
    "filesystem.workspace",
    "http"
  ]
}
```

| Field | Required | Behavior |
| --- | --- | --- |
| id | yes | 2–64 lowercase letters, digits, underscore or hyphen; must match directory |
| name | yes | display name |
| version | yes | workspace version string |
| entry | no | index.js by default; .js or .mjs |
| description | no | workspace description |
| authors | no | string array |
| permissions | no | capability id array |
| nativeMode | no | false by default |
| minimumNexora | no | minimum compatible Nexora semantic version; enforced before startup |
| dependencies | no | workspace id to exact, >=, ^, ~ or wildcard version constraint; enforced before startup |

## Capabilities

| Capability | Surface |
| --- | --- |
| minecraft.players | on, server, Player access |
| minecraft.world | Reserved for world API expansion |
| minecraft.entities | Reserved for entity API expansion |
| minecraft.inventory | item, inventory and GUI items |
| minecraft.commands | command |
| minecraft.packets | Reserved for packet providers |
| database | database |
| http | http |
| filesystem.workspace | storage |
| network.websocket | Reserved for workspace WebSocket providers |
| native.java | Unrestricted Java host lookup; Native Mode only |
| native.paper | native.paper and native.plugin; Native Mode only |
