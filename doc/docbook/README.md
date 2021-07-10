# Document

## enviroment version

```bash
$node -v
v14.4.0

$gitbook --version
CLI version: 2.3.2
GitBook version: 3.2.3
```

## 次やることmemo

## Memo

コマンドラインツールは、global に add するのがお約束。

一番の参考サイト
[URL](https://qiita.com/ikkei12/items/0f0c2d95bdd3b54d6bac)

参考サイト
[URL](https://zenn.dev/koduki/articles/430ba33bb8b8f6)

参考サイト2
[URL](https://zenn.dev/ririli47/articles/f8d12ad890ca4d9c615b)

## node version固定

[URL](https://qiita.com/suin/items/994458418c737cc9c3e8)

## Concept

## 作成予定機能

### login機能

### home page

### ポートフォリオ詳細 page

### 自身を紹介する page

### コードがどれくらいやっているのかを表す円グラフページ

## firebase

DBはサイトのURLとタイトルと画像URL
S3必要かな？firebaseに画像登録できるのであれば、そのまま

## 作成手順

```bash
$node -v

$npm install -g firebase-tools

$yarn create nuxt-app portfolio-web-site

以下プロジェクト作成時の選択
success Installed "create-nuxt-app@3.7.1" with binaries:
      - create-nuxt-app

create-nuxt-app v3.7.1
✨  Generating Nuxt.js project in portfolio-web-site
? Project name: portfolio-web-site
? Programming language: TypeScript
? Package manager: Yarn
? UI framework: Vuetify.js
? Nuxt.js modules: Axios - Promise based HTTP client
? Linting tools: ESLint, Prettier, Lint staged files, StyleLint, Commitlint
? Testing framework: Jest
? Rendering mode: Universal (SSR / SSG)
? Deployment target: Server (Node.js hosting)
? Development tools: jsconfig.json (Recommended for VS Code if you\'re not using typescript)
? Continuous integration: GitHub Actions (GitHub only)
? What is your GitHub username? naohito-t
? Version control system: Git
```

## memo (SPA・SSR・SSG)

[URL](https://qiita.com/nishinoshake/items/f42e2f03663b00b5886d)

Nuxt.jsではSPA・SSR・SSGの中から好きなものを選んで開発ができる
初期設定ではSSRで動作するようになっている。

SPA(Single Page Application)

- メリット
  実装しやすい
  サーバの準備が楽
  SPAは、最もシンプルに実装でき、ホスティング先の選択肢が多いのが魅力です。
  ドキュメントで、NetlifyやGitHub Pagesへのデプロイ方法が紹介されていますが、単にファイルをアップすればいいだけなので、ロリポップのようなレンタルサーバーでも動きます

- デメリット
  初期表示が遅い
  SEOに不安がある
  OGをページごとに設定ができない OGってなんだっけ

SSR(Single Side Rendering)

- メリット
  SPAの欠点を解消できる

- デメリット
  実装がSPAより面倒
  サーバーの準備が面倒

  初回のリクエストをサーバーサイドでレンダリングして返すため、SPAの欠点を補うことができます。一方で、レンダリングするためのサーバーと、SSRを考慮した実装が必要になります。
  ドキュメントで、HerokuやNowへのデプロイ方法が紹介されていますが、Node.jsが動作するサーバーを用意できればなんでも大丈夫です。インフラに弱い人にはこのハードルが高い気がしますが、インフラに強い人や、好きなPaaSがある人にとっては、SSRが魅力的な選択肢になると思います。

SSG(Static Site Generation)

- メリット
  SPAの欠点を解消できる
  **サーバーの準備が楽**
  SSRよりも速い
  更新が少ないWebサイト
  ドキュメントやブログ

- デメリット
  実装が少し面倒
  用途が限られる

各ルートのHTMLをあらかじめ生成するため、SSRよりもレスポンスが速いのが魅力です。また、静的ファイルを生成するおかげで、SPAと同じようにホスティング先の選択肢が広がります。

生成時にはサーバーサイドでレンダリングすることになるので、SSRを考慮した実装が必要になるのと、SSGには向き不向きがあるので、Webサイトの要件を考えて慎重に選択する必要があります。

## firebase

firebase project name
portfolio-web-site-revo

firestore Database
asia-northeast1 (東京)



## doc

[URL](https://qiita.com/minato-naka/items/3b0bcf0788a2150f3171)

## README 作成手順

[参考URL](https://zenn.dev/mebiusbox/articles/703e934c78fa20)

### gitbookについて

GitBook は、Markdown形式で作成した文章を HTML形式、PDF形式、ePub形式などの電子ブックを簡単に作ることができる。
GitBook は、クラウドサービスですが、
gitbook-cli を利用して、スタンドアロンで生成する環境を構築できます。

### gitbookインストール

グローバルにgitbook-cliをインストールする
```bash
$npm install -g gitbook-cli

インストール後、version確認
$ gitbook --version
CLI version: 2.3.2
GitBook version: 3.2.3

インストール後gitinit
$gitbook init
README.md と SUMMARY.mdが作成される

$gitbook build


```

