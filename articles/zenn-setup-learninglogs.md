---
title: "Zennのセットアップ。VS Codeでいい感じにコンテンツ管理する方法"
emoji: "🙆"
type: "idea" # tech: 技術記事 / idea: アイデア
topics: ["zenn"]
published: true
---

# Zennのセットアップ
技術学習のログをzennで残していくという目標定義ができたので、環境を整えていきます。
今回は学習内容の主が機械学習とかPythonということもあり、学習ログはZennで書いていくことにする。

ひとまず、Zennをgithub管理できるようにしていく。
正直なところ、あえてgithub連携する強い理由がエンジニアでもない僕にはないかもしれないが、そっちの方がかっこいいと思ったのでやってみた。

基本的には公式ドキュメント通りに進めていくだけでよいので、下記のURLを見ながらセットアップする。ZennとGitHubリポジトリを連携すると、ローカルで作成した.mdファイルをpushするだけで自動でzenn本体に記事をデプロイしてくれる。そこから編集も可能で非常にやりやすい。
https://zenn.dev/zenn/articles/connect-to-github


[Zenn CLI](https://zenn.dev/zenn/articles/install-zenn-cli)がめちゃ便利で、たとえば下記のコマンドでローカルでのプレビューを確認しながら記事作成ができたり。しかもホットリロード。

````
% npx zenn preview
````

ローカルのエディターでコンテンツ作成したり編集して、githubでコンテンツ管理するの結構いいかもしれないと改めて思いました。

# VS Codeで記事を作成・管理する

new articleを作るときにslugのオプションを設定する。一度作成した後は変更ができない仕様。
````
% npx zenn new:article --slug xxxxx
````
