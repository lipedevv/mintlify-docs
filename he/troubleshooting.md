---
title: "פתרון תקלות ורשימת בדיקות לייצור"
description: "אם שינוי נדחה, תקנו את אזהרת ה-Workspace הראשונה ואל תמחקו revisions. עצרו תהליך ישן כשהפורט תפוס, אל תריצו שני Paper על אותו עולם והשתמשו ב-nogui ב-Windows."
icon: wrench
---

<div dir="rtl">

# 🧰 פתרון תקלות ורשימת בדיקות לייצור

## Production checklist

לפני ייצור: גבו workspaces/storage, בדקו הפעלה/עצירה, הרשאות, מלאי מלא ויתרה חסרה, הגנו על ה-token ובדקו בדיוק את גרסת Paper המפורסמת.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.

</div>
