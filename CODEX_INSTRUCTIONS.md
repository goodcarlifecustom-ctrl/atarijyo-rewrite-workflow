# Codexへの指示

このリポジトリでは、30記事を一括処理せず、1記事ずつタスク詳細欄にHTMLを貼り付けて簡易リライトします。

## 重要

- zip内に article.html はありません
- 記事HTMLはCodexのタスク詳細欄に貼られた【現在の記事HTML】を使用してください
- 1タスクにつき1記事だけ処理してください
- 複数記事を一括処理しないでください

## 参照するファイル

- prompts/common_rewrite_prompt.md
- prompts/decoration_prompt.md
- prompts/wp_safety_rules.md
- prompts/output_format.md
- templates/task_input_template.md
- data/internal_links.csv
- data/affiliate_items.csv
- data/authority_links.csv

## 出力

- output/rewrite_report.md
- output/rewrite_review.html
- output/rewritten.html
- output/delete_suggestions.md
