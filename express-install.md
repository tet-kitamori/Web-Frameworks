## Express フレームワークのインストール

アプリケーション開発するフォルダを以下では、express-app とする。

### Express ジェネレータを利用しない場合
以下のようにして、express実行用のnodeモジュールをインストール

```
> mkdir express-app     // 作用用フォルダ作成
> cd express-app        // 作業用フォルダに移動
> npm init -y
> npm install express   // express 用のnode_modules
```
まだ、実行できるJSファイルがないので、次のようなindex.jsを作る
```
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
  res.send('Hello, Express!');
});

app.listen(port, () => {
  console.log(`Server running at localhost:3000`);
});
```
コマンドプロンプト、または、ターミナルから
```
> node index.js
```
としてサーバを起動する。
ブラウザから `http://localhost:3000` とすると'Hello Express!'が
表示される。　
正常に動作すれば、Expressが正常にインストールされているので、
これをベースにアプリケーションを開発する。

### Express ジェネレータを利用する場合

express ジェネレータを使用すると、フォルダ構成も最初からできており、
基本的なパッケージと最小限の実行ファイルが用意されてます。

express ジェネレータをインストールするには、以下のようにします。
```
> npm install -g express-generator
```

環境によっては、インストール時に管理者権限でないと成功しない場合が
あります。

Expressジェネレータのインストールが済んでいれば、
```
> express --view=ejs express-app
> cd express-app
> npm install
```
で、Expressフレームワークのインストールは完了です。
`> npm start` とするとサーバが起動されます。
ブラウザから `http://localhost:3000` とすると'Express'が
表示される。　

