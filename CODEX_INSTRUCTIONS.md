# Codexへの作業指示

このzip内のファイルを使って、SEOリライト用の分析・リライト・HTML出力を実行してください。

## 実行目的

Search Console、Ahrefs、SERP、現在記事HTMLをもとに、検索意図に合うように記事をリライトし、SWELL向けに装飾したHTMLを出力する。

## 実行ステップ

1. config.ymlを読み込む
2. article/article.htmlからtitle、h1、h2、h3、本文を抽出する
3. data/search_console.csvを読み込む
4. クリック数・表示回数・CTR・掲載順位を確認する
5. 現在記事のtitle、見出し、本文に不足しているKWを抽出する
6. data/ahrefs_organic_keywords.csvがあれば読み込む
7. GSCとAhrefsのKWを照合し、追加優先度を決める
8. serp/serp_headings.mdを読み込み、上位サイトにあって現記事に不足している要素を抽出する
9. 競合見出しをそのままコピーせず、独自見出しとして追加案を作る
10. 既存のSWELLブロック、ショートコード、アフィリエイトリンク、広告タグを壊さずにリライトする
11. prompts/decoration_prompt.mdに沿って装飾する
12. output/rewrite_report.mdを出力する
13. output/rewrite_review.htmlを出力する
14. output/rewritten.htmlを出力する
15. output/delete_suggestions.mdを出力する

## 出力ファイル

### output/rewrite_report.md

以下を含める。

- GSC分析結果
- Ahrefs分析結果
- SERP分析結果
- 追加したKW
- 見出しに追加したKW
- 本文に追加したKW
- 追加見出し
- 内部リンク追加案
- 公的リンク追加案
- アフィリエイト導線の改善案

### output/rewrite_review.html

確認用HTML。
追加・変更箇所に色付けする。

例：

<span class="rewrite-added">追加箇所</span>
<span class="rewrite-modified">修正箇所</span>

### output/rewritten.html

WordPress下書き投入用HTML。
色付けタグは削除する。

### output/delete_suggestions.md

削除候補を理由付きで提案する。
自動削除はしない。

## 絶対に守るルール

- 既存記事を更新しない
- WordPressに投稿する場合は新規下書きのみ
- statusはdraft固定
- publishは禁止
- futureは禁止
- 本体サイトには投稿しない
- 許可されていないURLなら処理を停止する
- 色付けHTMLをWordPress投入用HTMLに混ぜない
- アフィリエイトリンク、広告タグ、ショートコード、SWELLブロックを壊さない
- 競合サイトの見出し・本文をそのままコピーしない
- KWを不自然に詰め込まない
