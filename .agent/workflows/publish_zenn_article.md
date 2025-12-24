---
description: Zenn記事を公開する
---

Zenn記事を公開するための標準的な手順です。

## 1. 公開設定の変更
対象の記事ファイルのフロントマターで `published: false` を `true` に書き換えます。

## 2. GitHubへのプッシュ
変更をコミットしてリモートリポジトリに送信します。

// turbo
1. 修正した記事をステージングします。
   ```bash
   git add articles/[filename].md
   ```
2. コミットメッセージを作成します。記事の内容に基づいた適切なメッセージを使用してください（例：`docs: publish [article title]`）。
   ```bash
   git commit -m "docs: publish [meaningful message]"
   ```
3. GitHubにプッシュします。
   ```bash
   git push origin HEAD
   ```

## 3. 公開確認
GitHubへのプッシュ後、Zennのウェブサイト上で記事が正しく公開されているか確認する。