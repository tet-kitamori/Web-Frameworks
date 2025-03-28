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
3. Webブラウザで `http:\\localhost:3000` とすると Vue-cli のページが表示される。
