# alg.tus-ricora.com

[![Generator is Hugo](https://img.shields.io/badge/Generator-Hugo-ff4088?&logo=hugo)](https://github.com/gohugoio/hugo)
[![GitHub Pages](https://github.com/RICORA/alg.tus-ricora.com/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/RICORA/alg.tus-ricora.com/actions/workflows/gh-pages.yml)

## Overview

このリポジトリは[RICORA Programming Teamのブログ](https://alg.tus-ricora.com/)を管理するためのものです。ブログの編集やローカルでの閲覧方法については[このリポジトリのWiki](https://github.com/RICORA/alg.tus-ricora.com/wiki)を参照してください。

## Contribution

ブログの新規ページを作成したい/編集をしたいときは、まず[Wiki](https://github.com/RICORA/alg.tus-ricora.com/wiki)を読んでください。
疑問があったら[Issues](https://github.com/RICORA/alg.tus-ricora.com/issues)に投げてください。

### Branchの命名規則

[ここ](https://github.com/RICORA/alg.tus-ricora.com/wiki/%E3%83%96%E3%83%AD%E3%82%B0%E3%81%AE%E7%B7%A8%E9%9B%86#branch%E3%81%AE%E5%91%BD%E5%90%8D%E8%A6%8F%E5%89%87)にも書いてありますが、以下のようにBranchを命名していただけると管理しやすく助かります。

|作業内容|Branch名|
|:-:|:-:|
|ブログ記事の新規作成と編集|`post/(ページタイトル)`|
|固定ページの新規作成と編集|`page/(ページタイトル)`|
|テーマの編集や機能追加等|`feature/(機能名等)`|

### ファイル命名規則

- アルファベットの小文字と数字のみ使うようにしましょう。

### コードスタイル

Pull Requestを送る前に以下のコマンドでLintを行い、エラーが出ていないかを確認してください。実行には[Node.js](https://nodejs.org/ja/)が必要です。

```sh
npm install # 初回のみ実行してください。node_modules/が生成されます。
npm run format
npm run lint
```

Linterの設定は`.markdownlint-cli2.jsonc`と`.textlintrc.json`に記述してあります。記事を作成する上で不都合が生じた場合は、適宜修正してください。
