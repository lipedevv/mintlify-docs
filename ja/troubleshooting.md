---
title: "トラブルシューティングと本番チェック"
description: "変更が拒否されたら最初の Workspace 警告を修正し、リビジョンは削除しないでください。ポート使用中は古いプロセスを停止し、同じワールドに Paper を2つ起動せず、Windows では nogui を使用します。"
icon: wrench
---

## Production checklist

本番前に workspaces/storage をバックアップし、起動停止、権限、満杯のインベントリ、残高不足をテストし、トークンを保護し、告知した正確な Paper ビルドを検証してください。

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
