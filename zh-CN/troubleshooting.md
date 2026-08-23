---
title: "故障排除与生产检查"
description: "修改被拒绝时，修复第一条 workspace 警告，不要删除版本。端口占用时停止旧进程；不要让两个 Paper 实例使用同一世界；Windows 使用 nogui。"
icon: wrench
---

## Production checklist

上线前备份 workspaces/storage，测试启动停止、权限、满背包和余额不足，安全保存管理员令牌，并测试你声明支持的准确 Paper 构建。

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
