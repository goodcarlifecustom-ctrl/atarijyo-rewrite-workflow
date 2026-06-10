# Codexタスク詳細入力テンプレート

`prompts/common_rewrite_prompt.md`、`prompts/decoration_prompt.md`、`prompts/wp_safety_rules.md`、`prompts/output_format.md` の指示に従って、以下の1記事のみを簡易リライトしてください。

複数記事を一括処理しないでください。
このタスクの詳細欄に貼り付けた【現在の記事HTML】を対象記事のHTMLとして扱ってください。
zip内に article.html はありません。

---

## 対象記事

【記事URL】
ここに記事URLを入力

【メインKW】
ここにメインKWを入力

【サブKW】
ここにサブKWを入力

【記事の目的・メモ】
ここに任意で入力

---

## Search Consoleデータ

以下に、この記事に関係するSearch Consoleデータを貼ってください。

```csv
クエリ,クリック数,表示回数,CTR,掲載順位
ここに貼り付け
```

---

## Ahrefsデータ

Ahrefsデータがある場合のみ貼ってください。
ない場合は「なし」と入力してください。

```csv
Keyword,Volume,KD,Traffic,Position,URL,Parent topic
ここに貼り付け
```

---

## 上位サイト・SERPメモ

ある場合のみ貼ってください。
ない場合は「なし」と入力してください。

```text
1位：
URL：
タイトル：
H2/H3：
特徴：

2位：
URL：
タイトル：
H2/H3：
特徴：
```

---

## 現在の記事HTML

以下にWordPress編集画面から取得したHTMLを貼ってください。

```html
ここに現在の記事HTMLを貼り付け
```

---

## 出力してほしいもの

- output/rewrite_report.md
- output/rewrite_review.html
- output/rewritten.html
- output/delete_suggestions.md

## 特に守ってほしいこと

- 既存記事は更新しない
- WordPressに投稿する場合は新規下書きのみ
- アフィリエイトリンクを壊さない
- SWELLブロックを壊さない
- ショートコードを壊さない
- 変更箇所の色付けは確認用HTMLだけ
- WordPress投入用HTMLからは色付けを削除
