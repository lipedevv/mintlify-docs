---
title: "自动重载"
description: "保存 workspace.json、.js、.mjs 或本地 .json 会触发验证。候选版本在隔离环境准备，并在 Paper 主线程替换；失败时继续运行最后一个健康版本。"
icon: refresh-cw
---

> Saving `workspace.json`, `.js`, `.mjs` or local `.json` files is enough. There is no Deploy Workspace command.

修改被拒绝时，修复第一条 workspace 警告，不要删除版本。端口占用时停止旧进程；不要让两个 Paper 实例使用同一世界；Windows 使用 nogui。
