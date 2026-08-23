---
title: "Workspace 清单"
description: "只有 id、name、version 必填；entry 默认为 index.js。必须声明脚本使用的全部能力。原生模式同时需要服务器启用和 workspace 选择加入。"
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
