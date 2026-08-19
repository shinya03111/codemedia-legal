# codemedia-legal

CodeMedia の**全アプリのプライバシーポリシーの正本**を GitHub Pages で公開するリポジトリ。
ポリシー本文はここ以外に置かない（各アプリの LP / サポートページからはここへリンクする）。

公開 URL:

| ページ | URL |
|---|---|
| トップ(一覧) | https://shinya03111.github.io/codemedia-legal/ |
| 精算ノート | https://shinya03111.github.io/codemedia-legal/splitbill/ |
| バケットリスト | https://shinya03111.github.io/codemedia-legal/bucketlist/ |
| つみにち | https://shinya03111.github.io/codemedia-legal/tsuminichi/ |
| いいことみっけ | https://shinya03111.github.io/codemedia-legal/iikoto/ |
| ポスネタ | https://shinya03111.github.io/codemedia-legal/posneta/ |
| よみかえし | https://shinya03111.github.io/codemedia-legal/yomikaeshi/ |
| キフログ | https://shinya03111.github.io/codemedia-legal/kifulog/ |
| おかん天気 | https://shinya03111.github.io/codemedia-legal/okantenki/ |
| ミタテ | https://shinya03111.github.io/codemedia-legal/mitate/ |

App Store Connect / Google Play Console のプライバシーポリシー URL には、
上記のアプリ別 URL を登録する。サポート URL / マーケティング URL は別物なので、
各アプリのサイト（posneta-support / iikoto-mikke など）をそのまま使う。

問い合わせ先は全ページ `codemedia.app@gmail.com` に統一。

## 移行状況（2026-08-09 時点）

| アプリ | ストアに登録中の URL | 対応 |
|---|---|---|
| 精算ノート (iOS) | 旧 Notion URL | 全バージョン READY_FOR_SALE のため今は変更不可（409）。**次バージョン作成時に `splitbill/` へ差し替える** |
| 精算ノート (Android) | `splitbill/` | 対応済み |
| バケットリスト (iOS) | `bucketlist/` | 対応済み |
| つみにち | 未提出 | 最初から `tsuminichi/` を登録する |
| いいことみっけ | `iikoto-mikke/privacy/` | 審査中のため据え置き。**審査通過後に `iikoto/` へ差し替え、旧ページは転送にする** |
| ポスネタ (iOS) | `posneta/` | 対応済み |
| ポスネタ (Android) | 未登録 | 最初から `posneta/` を登録する |

## 構成

素の静的 HTML（Jekyll を通さないため `.nojekyll` を置いている）。
外部リクエストは一切なく、`style.css` だけを共有している。
ダークモードは `prefers-color-scheme` で自動対応。

```
index.html          一覧
style.css           共通スタイル
splitbill/index.html
bucketlist/index.html
tsuminichi/index.html
iikoto/index.html
posneta/index.html
```

## 更新するとき

内容を書き換えたら、各ページの「最終更新」日付も更新して push する。
push の1〜2分後に Pages へ反映される。

新しいアプリを追加する場合は、ディレクトリを作って `index.html` を置き、
`index.html`（トップ）のアプリ一覧にリンクを追加する。
