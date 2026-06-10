# Codex貼り付け用：1記事テストリライト

以下の1記事だけを簡易SEOリライトしてください。
GitHub内のCSVやarticle.htmlは読まないでください。このタスク本文にある情報だけを使ってください。
今回はWordPress投稿は行わず、HTML出力までにしてください。既存記事は絶対に更新しないでください。

## 対象記事

記事URL：
https://www.atarijo.com/media/sapporo-sexfriend/

メインKW：
札幌 セフレ

サブKW：
札幌 セフレ 出会い

## Search Consoleデータ

期間：過去28日間
検索タイプ：ウェブ
対象ページ：https://www.atarijo.com/media/sapporo-sexfriend/

| クエリ | クリック数 | 表示回数 | CTR | 掲載順位 |
|---|---:|---:|---:|---:|
| 札幌 セフレ | 2 | 67 | 2.99% | 11.73 |
| セフレ 札幌 | 0 | 15 | 0% | 10.6 |
| 札幌セフレ | 0 | 12 | 0% | 9.42 |

| ページ | クリック数 | 表示回数 | CTR | 掲載順位 |
|---|---:|---:|---:|---:|
| https://www.atarijo.com/media/sapporo-sexfriend/ | 9 | 173 | 5.2% | 9.75 |

Ahrefsデータ：
なし

上位サイトメモ：
なし

## リライト方針

1. Search Consoleで反応がある「札幌 セフレ」「セフレ 札幌」「札幌セフレ」を、title案・導入文・見出し・本文に自然に反映してください。
2. 不自然なKW詰め込みはしないでください。
3. 全面リライトではなく、テスト用の簡易リライトにしてください。
4. 追加見出しは最大3個までにしてください。
5. 既存のHTML構造、画像、表、内部リンク、外部リンク、ショートコード、アフィリエイトリンク、SWELL系の装飾はできる限り保持してください。
6. 既存のマーカーは一度見直し、重要箇所だけに整理してください。
7. 「この記事でわかること」リスト、H2/H3アンカーリンク、cap_box装飾、段落分割、マーカー装飾を整えてください。
8. 既にあるid属性は原則保持してください。重複やリンク切れがあれば修正してください。
9. 「5つの方法」と本文で6つ紹介している箇所、9選とリストが10件以上ある箇所など、件数のズレがあれば修正してください。
10. 誤字・不自然な表現があれば修正してください。例：「出う」「演出し Lましょう」など。
11. 相手の弱みにつけ込む、未成年・金銭・強引な誘導につながる表現は避け、成人同士の合意・安全・相手への尊重を明確にしてください。

## 装飾ルール

- 最初のH2直前に「この記事でわかること」のアンカーリンク付きリストを設置・整理してください。
- H2配下に複数H3がある場合、必要に応じてH3へのアンカーリンク付きリストを設置してください。
- 重要なリストは以下のcap_boxで囲んでください。ただし、全てのulを機械的に囲まないでください。

```html
<div class="swell-block-capbox cap_box is-style-onborder_ttl">
  <div class="cap_box_ttl"><span>ここにタイトル</span></div>
  <div class="cap_box_content">
    <ul>
      <li>リスト項目</li>
    </ul>
  </div>
</div>
```

- 長いpタグは、意味のまとまりごとに複数のpタグへ分割してください。
- ポジティブな重要箇所は以下の黄色マーカーを使ってください。

```html
<span class="swl-marker mark_yellow">強調する文章</span>
```

- 注意点・リスクなどのネガティブな重要箇所は以下を使ってください。

```html
<mark style="background-color:rgba(0, 0, 0, 0)" class="has-inline-color has-swl-deep-01-color">強調する文章</mark>
```

## 出力

以下の4ファイルを作成してください。

- output/rewrite_report.md
- output/rewrite_review.html
- output/rewritten.html
- output/delete_suggestions.md

rewrite_review.html：
変更箇所に以下のような色付けを入れてください。

```html
<span class="rewrite-added">追加箇所</span>
<span class="rewrite-modified">修正箇所</span>
```

rewritten.html：
WordPress下書き投入用です。rewrite-added / rewrite-modified / 凡例CSSなど、確認用の色付けは削除してください。
SWELL装飾、cap_box、アンカーリンク、マーカーは残してください。

delete_suggestions.md：
削除候補を理由付きで提案してください。自動削除はしないでください。

## 現在の記事HTML

この下に、WordPress編集画面の本文HTMLだけを貼ってください。

```html
ここに本文HTMLを貼る
```

