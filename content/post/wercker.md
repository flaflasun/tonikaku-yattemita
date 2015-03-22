+++
date = "2015-03-22T23:03:55+09:00"
draft = false
title = "Werckerを使ってHugoのデプロイ自動化"

+++

### Werckerについて

[Wercker](http://wercker.com/)は無料で使えるCIツールです。  
GitHubへのPushにフックしてアプリケーションのテスト、ビルド、デプロイすることが出来ます。  

### Werckerを使ってGitHub Pagesへデプロイ

今回はHugoで作成しているブログのデプロイを自動化するためにWerckerを使ってみました。  

Hugoについては[こちら](hugo/index.html)  

#### Werckerを選んだ理由

理由は単純に公式サイトで紹介されているのがWerckerだったからです。  

#### Wercke導入までの流れ

Wercker導入の手順はHugoの公式サイトに記載されているので、
概要だけ紹介しようと思います(Hugoインストール、GitHubリポジトリ作成は除く)。  

1. Hugoでブログを作成(利用するテーマの .git は削除する必要あり)
2. Werckerに[登録](http://wercker.com/)
3. WerckerとGitHubアカウントを紐付ける
4. WerckerにGitHubプロジェクトを登録
5. Wercker.yml作成(ビルドとデプロイ設定を作成)
6. Werckerにデプロイする対象(GitHubのブランチ)を選択
7. GitHubにPushする

ここまで、設定すればあとはGitHubにPushするたびに
Hugoのビルド、デプロイまでWerckerが自動でやってくれます。  

この記事ではざっくり書いてますが、
公式サイトの手順はしっかり書かれているので、
そちらを参考にするのがいいです。  
[Automated deployments with Wercker](http://gohugo.io/tutorials/automated-deployments/)  

### Werckerを導入してみて

Wercker導入後はわざわざビルドやデプロイをする必要がなくなり、とても快適です。
導入自体も公式サイトの手順がしっかりしているので、割りと簡単に出来ました。
今回はブログのデプロイ自動化でしたが、
無料で簡単に使えるので他のことにも使ってみたいなと感じさせるサービスでした。  
