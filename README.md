# peterpan

Markdown で店舗案内やメニューの更新ができるサンプルです。`docs/` のディレクトリをご覧ください。

- https://phpeter-pi.github.io/peterpan/

## 仕組み

`docs/index.html` の Javascript が、同じ階層にある Markdown ファイルを読み込み、HTML にパースして表示します。

### Markdown to HTML パーサー

- [MDwiki](http://dynalon.github.io/mdwiki/#!index.md) [v0.6.2](https://github.com/Dynalon/mdwiki/releases/tag/0.6.2) @ GitHub
- 使われているライブラリ
  - jQuery v1.8.3
    - jquery.colorbox.js
  - Bootstrap v3.0.0
  - highlight v7.3
  - MDwiki.js

### 参考文献

- https://qiita.com/sta/items/a1ee3537ce6e7cfe34a8 @ Qiita

## 利用時の注意事項

MDwiki の利用規約に基づき、必ず LICENSE.txt および GPLv3.txt も一緒に設置してください。
