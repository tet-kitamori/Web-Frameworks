インストール
# WEB Framework
Javascript エンジンの node.js が公開されて以来、
node.js をベースにしたエコシステムが構成され、多くの
人が利用しています。

数多くのアプリケーションフレームワークがあり、それぞれの特徴があります。
[主なアプリケーションフレームワーク](./frameworks.md)
これらのアプリケーションフレームワークは公開され、日々、改善・機能アップ
がなされています。

アプリケーションフレームワークを最初に使うとき、書籍やネットの記事、
Copilotなど参考に試して見ますが、うまく行かないこともあるし、
インストールのやり方が複数あって、迷ってしまいます。

このリポジトリでは、node.js ベースのアプリケーションフレームワークを
インストールする時の方法に関して記載します。

ここでの前提条件は、node.js と npm はインストールされており、
nodeパッケージの管理は、npm を用いるものとします。

職場のPCがセキュリティ規約上使用できない場合は、個人の
PCまたは、Raspberry Pi や Jetson などの Linux 基板等で
試してください。

## Express のインストール

Expressのインストール方法は、
[Express のインストール](./express-install.md)

## React のインストール

Reactのインストール方法は、
[React のインストール](./react-install.md)

## Vue.js のインストール

Vue.jsのインストール方法は、
[Vue.js のインストール](./vuejs-install.md)

## Next.js のインストール

Next.jsのインストール方法は、
[Next.js のインストール](./nextjs-install)

## Nuxt.js のインストール

Nuxt.jsのインストール方法は、
[Nuxt.js のインストール](./nuxtjs-install.md)


## **注記**
ここに、記載された内容は kitamori が実際に動作確認した内容ですが、
動作環境により期待通りに動かせない可能性もあります。

アプリケーションフレームワークは、専用のジェネレータを使用した方が
開発が楽です。　このジェネレータをインストールする場合に、管理者権限
でないと成功しない場合があります。
多くの場合、Windows PC では、コマンドプロンプト、または、PowerShell 
を管理者権限で起動してインストールします。
Linux の場合は、`$ sudo npm install XXXXXXXXXX` でインストールします。
困った時は、Copilot！

Visual Studio Code を開発環境として利用するとき、ターミナルから
スクリプトを実行できない場合は、PowerShellの権限（実行ポリシー）を
確認してください。 
PowerShell の上からであれば、`Get-ExecutionPolicy -List`　で確認できます。
権限は、'Restricted', 'AllSigned', 'RemoteSigned', 'Unrestricted',
'Bypassed', 'Undefined' の6種類があります。
権限が 'Ristricted' になっているとスクリプトの実行ができません。 
```
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser -Force
```
で、カレントユーザの権限を 'RemoteSigned'に変更できます。
 'RemoteSigned'　では、ローカルで作成されたスクリプトは制限なく実行できますが、
 インターネットから取得したスクリプトには信頼された署名が必要です。
詳細は、Copilot！
