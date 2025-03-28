## Nuxt.js のインストール
### ジェネレータを使わずに最小限のインストールを行う場合

1. 作業用のフォルダを作成する。
2. ターミナルで作業用フォルダに移動し、Nuxt.js を以下のようにインストール。
```
> npm init
> npm install --save nuxt
```
3. pages フォルダを作成し、次のような index.vue ファイルを作成する。
```
<template>
  <div>
    <h1> Hello Nuxt! </h1>
  </div>
</template>
```
4. package.json の "scripts" に、Nuxt 実行用コマンド追加
```
"scripts": {
    "dev": "nuxt dev",     // 追加
    略
}
```
5. ターミナルで `npm run dev` としてサーバ起動。
6. Webブラウザで `http:\\localhost:3000` とすると 'Hello Nuxt!'と表示される。

### Vue-cli を使ってインストールする。

まず、Vue-cli　をグローバルのパッケージとしてインストールする。
```
> npm install -g @vue/cli
```
vue-cli がインストールされていれば、個々のプロジェクトは以下のようにして作成できる。
1. `vue init nuxt-community/starter-template vue-cli-app` として
テンプレートからプロジェクトを作成する。
いくつかの質問が来るので、適当に返答してください。
2. 作成されたフォルダに移動して、
```
> npm install      // 必要なパッケージをインストール
> npm run dev      // nuxt 実行
```
3. Webブラウザで `http:\\localhost:3000` とすると Vue-cli紹介ページが表示される。

