---
title: "Устранение неполадок и проверка перед выпуском"
description: "При отклонении сохранения исправьте первое предупреждение workspace и не удаляйте ревизии. Освободите занятый порт, не запускайте два Paper для одного мира и используйте nogui в…"
icon: wrench
---

## Production checklist

Перед продажей создайте резервные копии, проверьте запуск/остановку, права игрока и консоли, полный инвентарь и нехватку средств, защитите токен и тестируйте заявленную сборку Paper.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
