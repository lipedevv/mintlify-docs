---
title: "โหลดซ้ำอัตโนมัติ"
description: "การบันทึก workspace.json, .js, .mjs หรือ .json ภายในจะเริ่มตรวจสอบ รุ่นใหม่ถูกเตรียมแบบแยกและสลับบน main thread ของ Paper หากล้มเหลว รุ่นที่สมบูรณ์ล่าสุดยังทำงาน"
icon: refresh-cw
---

> Saving `workspace.json`, `.js`, `.mjs` or local `.json` files is enough. There is no Deploy Workspace command.

หากการแก้ไขถูกปฏิเสธ ให้แก้ warning แรกและอย่าลบ revision หาก port ถูกใช้ให้หยุด process เก่า ห้ามเปิด Paper สองตัวกับ world เดียวกัน และใช้ nogui บน Windows
