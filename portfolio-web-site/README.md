# portfolio-web-site

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Special Directories

You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

### `assets`

The assets directory contains your uncompiled assets such as Stylus or Sass files, images, or fonts.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

### `components`

The components directory contains your Vue.js components. Components make up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

日本語訳
componentsディレクトリには、Vue.jsのコンポーネントが格納されています。コンポーネントは、ページのさまざまな部分を構成するもので、ページやレイアウト、さらには他のコンポーネントに再利用したり、インポートしたりすることができます。

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/components).

### `layouts`

Layouts are a great help when you want to change the look and feel of your Nuxt app, whether you want to include a sidebar or have distinct layouts for mobile and desktop.

日本語訳
レイアウトは、サイドバーを入れたり、モバイル用とデスクトップ用で異なるレイアウトにしたりと、Nuxtアプリの見た目を変えたいときに大きな助けとなります。

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts).


### `pages`

This directory contains your application views and routes. Nuxt will read all the `*.vue` files inside this directory and setup Vue Router automatically.

日本語訳
このディレクトリには、アプリケーションのビューとルートが含まれています。Nuxtは、このディレクトリ内のすべての `*.vue` ファイルを読み込んで、Vue Routerを自動的に設定します。

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/get-started/routing).

### `plugins`

The plugins directory contains JavaScript plugins that you want to run before instantiating the root Vue.js Application. This is the place to add Vue plugins and to inject functions or constants. Every time you need to use `Vue.use()`, you should create a file in `plugins/` and add its path to plugins in `nuxt.config.js`.

日本語訳
pluginsディレクトリには、ルートのVue.jsアプリケーションをインスタンス化する前に実行したいJavaScriptプラグインが含まれています。これは、Vueプラグインを追加したり、関数や定数を注入するための場所です。Vue.use()` を使用する必要がある場合は、`plugins/` にファイルを作成し、そのパスを `nuxt.config.js` の plugins に追加する必要があります。

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins).

### `static`

This directory contains your static files. Each file inside this directory is mapped to `/`.

Example: `/static/robots.txt` is mapped as `/robots.txt`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/static).

### `store`

This directory contains your Vuex store files. Creating a file in this directory automatically activates Vuex.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/store).
