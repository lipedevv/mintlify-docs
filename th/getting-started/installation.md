---
title: "การติดตั้ง"
description: "เป้าหมายที่รองรับคือ Paper 1.21.8 และ Java 21 ขึ้นไป ใช้ VS Code เฉพาะเมื่อต้องการสถานะสดหรือดูตัวอย่าง GUI ผ่าน Nexora Connect"
icon: package
---

หยุดเซิร์ฟเวอร์ คัดลอก NexoraEngine.jar ไปยัง plugins เริ่มด้วย java -jar server.jar nogui เก็บ token เริ่มต้นที่แสดงเพียงครั้งเดียว และวาง Workspace ใน plugins/NexoraEngine/workspaces

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
