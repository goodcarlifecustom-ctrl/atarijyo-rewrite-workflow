# WordPress下書き投稿時の安全ルール

WordPress投稿を行う場合は、以下を必ず守ってください。

## 絶対条件

- 既存記事は絶対に更新しない
- WordPressには必ず新規下書きとして作成する
- status は必ず draft
- publish / future / private は禁止
- 既存記事の本文差し替えは禁止
- 既存記事の更新APIは使わない
- PUT /wp/v2/posts/{id} は禁止
- POST /wp/v2/posts/{id} による既存記事更新は禁止
- 新規下書き作成以外は禁止

## 投稿前チェック

投稿前に以下を確認してください。

- draft_only = true
- allow_update_existing = false
- status = draft
- target_base_url が許可されたURLである
- forbidden_base_url に一致していない
- rewritten.html から色付けタグが削除されている
- review用HTMLをWordPressに投入していない

## 停止条件

以下に該当する場合は投稿処理を停止してください。

- 本体サイトURLが指定されている
- target_base_url が不明
- status が draft 以外
- 既存post_idを更新しようとしている
- rewrite_review.html を投稿しようとしている
- アフィリエイトリンクやショートコードが破損している可能性がある
