# Peter pan

Markdown でサイトの更新ができるサンプルです。「ホームに追加」ボタンの実装もされています。

**SEO（検索エンジン）向けではありません**。常連客などに URL を教えて見てもらうためのものです。本日のメニューや来客状況などに利用します。

- サンプルデータ： [`docs/` ディレクトリ](docs/)
- 動作サンプル： https://phpeter-pi.github.io/peterpan/

## 仕組み

`docs/index.html` の Javascript が、同じ階層にある Markdown ファイルを読み込み、HTML にパースして表示します。

また、「ホームに追加」ボタンは ServiceWorker 利用しています。

### Markdown to HTML パーサー

- [MDwiki](http://dynalon.github.io/mdwiki/#!index.md) [v0.6.2](https://github.com/Dynalon/mdwiki/releases/tag/0.6.2) @ GitHub
- 使われているライブラリ
  - jQuery v1.8.3
    - jquery.colorbox.js
  - Bootstrap v3.0.0
  - highlight v7.3
  - MDwiki.js

### 変更が必要なファイル

- `index.html`: `<title>` タグを店舗名に表示
- `config.json`: `index.html` のタイトルと同じ店舗名に変える
- `manifest.json`: `name` と `short_name` を、店舗名と「ホームに追加」時のアイコン表示名に変える
- `icon_144x144.png`: 「ホームに追加」時のアイコン画像に変える
- `navigation.md`: タイトル行（`#` 付きの先頭行）を店舗名に変える

### 参考文献

- [Markdown を HTML ファイル一つで Wiki っぽく見せる MDWiki が便利な件](https://qiita.com/sta/items/a1ee3537ce6e7cfe34a8) @ Qiita
- [「ホーム画面に追加」からはじめる『PWA(Service Worker)』](https://qiita.com/narikei/items/4240f03542f29e313989) @ Qiita

## 利用時の注意事項

MDwiki の利用規約に基づき、必ず LICENSE.txt および GPLv3.txt も一緒に設置してください。
