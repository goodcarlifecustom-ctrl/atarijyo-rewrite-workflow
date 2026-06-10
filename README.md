# SEOリライト用 input zip テンプレート

このzipは、Codex / GitHub Actions / ローカル実行でSEO記事リライトを進めるための入力ファイル一式です。

## 基本の流れ

1. Search Console CSVを読み込む
2. 現在記事HTMLと照合し、タイトル・見出し・本文に入っていないKWを抽出する
3. Ahrefsデータがあれば照合する
4. 検索結果・上位サイト見出しを確認する
5. リライトを実行する
6. 装飾プロンプトに沿ってSWELL向けに装飾する
7. 確認用HTMLとWordPress下書き投入用HTMLを分けて出力する
8. WordPressには必ず新規下書きとして投稿する
9. 本体記事は絶対に更新しない

## 最低限入れるファイル

- article/article.html
- article/article_url.txt
- data/search_console.csv
- prompts/decoration_prompt.md
- config.yml

## あると精度が上がるファイル

- data/ahrefs_organic_keywords.csv
- data/internal_links.csv
- data/affiliate_items.csv
- serp/serp_headings.md
- data/authority_links.csv

## 注意

WordPressログイン情報、APIキー、アフィリエイト管理画面のログイン情報はこのzipに入れないでください。
それらはGitHub Secretsや環境変数で管理してください。
