---
title: "Усунення проблем і перевірка production"
description: "Якщо зміну відхилено, виправте перше попередження й не видаляйте ревізії. Зупиніть старий процес при зайнятому порту, не запускайте два Paper для одного світу та використовуйте…"
icon: wrench
---

## Production checklist

Перед production створіть резервні копії, перевірте запуск/зупинку, права, повний інвентар і нестачу коштів, захистіть токен і тестуйте саме заявлений Paper build.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
