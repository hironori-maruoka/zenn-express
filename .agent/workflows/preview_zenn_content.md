---
description: Zennコンテンツをプレビューする
---
1. バックグラウンドで `npx zenn preview` コマンドを実行します。`WaitMsBeforeAsync` は 3000ms 程度に設定します。
2. サーバーの起動を数秒待ちます。
3. `browser_subagent` ツールを使用して `http://localhost:8000` を開きます。
4. プレビューが `http://localhost:8000` で起動したことをユーザーに通知します。
5. ユーザーが確認を終えたら、`send_command_input` ツール（`Terminate: true`）を使用してバックグラウンドプロセスを終了し、ポートを閉じます。
