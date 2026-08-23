---
title: "แก้ไขปัญหาและรายการตรวจสอบก่อนใช้งานจริง"
description: "หากการแก้ไขถูกปฏิเสธ ให้แก้ warning แรกและอย่าลบ revision หาก port ถูกใช้ให้หยุด process เก่า ห้ามเปิด Paper สองตัวกับ world เดียวกัน และใช้ nogui บน Windows"
icon: wrench
---

## Production checklist

ก่อนใช้งานจริงให้สำรอง workspaces/storage ทดสอบ start/stop, permission, inventory เต็มและเงินไม่พอ ป้องกัน token และทดสอบ Paper build ที่ประกาศให้ตรงกัน

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
