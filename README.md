# SEOリライト共通素材zip：タスク詳細HTML貼り付け運用版

1記事ずつCodexの「タスクの詳細」欄にHTMLを貼ってリライトする運用向けです。

## このzipの目的

- 毎回 article.html をzipに入れない
- 記事HTMLはCodexのタスク詳細欄に直接貼る
- zipには共通プロンプト、装飾ルール、安全ルール、入力テンプレート、共通CSVだけを入れる
- 1記事ずつ結果を確認しながら、30記事を安全に簡易リライトする

## 基本の使い方

1. このzipをGitHubリポジトリまたはCodex作業環境に置く
2. Codexのタスク詳細欄に `templates/task_input_template.md` の内容をコピーする
3. 記事URL、メインKW、Search Consoleデータ、Ahrefsデータ、現在の記事HTMLを貼る
4. 1記事だけリライトする
5. 出力された `rewrite_review.html` と `rewritten.html` を確認する
6. 問題があればプロンプトを修正して次の記事へ進む

## 重要

このzipには `article.html` は含めません。
記事HTMLは毎回、Codexのタスク詳細欄に貼り付けてください。

## 推奨出力

Codexには、1記事ごとに以下を出力させます。

- output/rewrite_report.md
- output/rewrite_review.html
- output/rewritten.html
- output/delete_suggestions.md

## 絶対に守ること

- 本体記事は絶対に更新しない
- WordPressには新規下書きのみ作成する
- `rewrite_review.html` の色付けタグをWordPress投入用HTMLに混ぜない
- SWELLブロック、ショートコード、広告タグ、アフィリエイトリンクを壊さない
- 競合サイトの見出しや本文をそのままコピーしない
