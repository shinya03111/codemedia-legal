# codemedia-legal

CodeMedia のアプリのプライバシーポリシーを GitHub Pages で公開するリポジトリ。

公開 URL:

| ページ | URL |
|---|---|
| トップ(一覧) | https://shinya03111.github.io/codemedia-legal/ |
| 精算ノート | https://shinya03111.github.io/codemedia-legal/splitbill/ |
| バケットリスト | https://shinya03111.github.io/codemedia-legal/bucketlist/ |

App Store Connect / Google Play Console のプライバシーポリシー URL には、
上記のアプリ別 URL を登録する。

## 構成

素の静的 HTML（Jekyll を通さないため `.nojekyll` を置いている）。
外部リクエストは一切なく、`style.css` だけを共有している。
ダークモードは `prefers-color-scheme` で自動対応。

```
index.html          一覧
style.css           共通スタイル
splitbill/index.html
bucketlist/index.html
```

## 更新するとき

内容を書き換えたら、各ページの「最終更新」日付も更新して push する。
push の1〜2分後に Pages へ反映される。

新しいアプリを追加する場合は、ディレクトリを作って `index.html` を置き、
`index.html`（トップ）のアプリ一覧にリンクを追加する。
