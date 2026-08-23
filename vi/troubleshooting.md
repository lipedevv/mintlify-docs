---
title: "Khắc phục lỗi và kiểm tra production"
description: "Nếu thay đổi bị từ chối, sửa cảnh báo workspace đầu tiên và không xóa revision. Dừng tiến trình cũ khi cổng bận, không chạy hai Paper cùng world và dùng nogui trên Windows."
icon: wrench
---

## Production checklist

Trước production: sao lưu workspaces/storage, thử khởi động/tắt, quyền, kho đầy và thiếu tiền, bảo vệ token và kiểm tra đúng build Paper đã công bố.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
