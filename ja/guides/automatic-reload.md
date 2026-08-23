---
title: "自動リロード"
description: "workspace.json、.js、.mjs、ローカル .json の保存で検証が始まります。候補リビジョンを隔離して準備し、Paper のメインスレッドで交換します。失敗時は最後の正常なリビジョンが継続します。"
icon: refresh-cw
---

> Saving `workspace.json`, `.js`, `.mjs` or local `.json` files is enough. There is no Deploy Workspace command.

変更が拒否されたら最初の Workspace 警告を修正し、リビジョンは削除しないでください。ポート使用中は古いプロセスを停止し、同じワールドに Paper を2つ起動せず、Windows では nogui を使用します。
