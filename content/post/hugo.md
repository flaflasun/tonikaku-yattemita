+++
date = "2015-03-09T20:54:33+09:00"
draft = false
title = "Hugoを使ってブログスタート"

+++

### Hugoを選んだ理由

HugoはGo言語で作られたサイトジェネレータです。  
詳細は先人が紹介しているので省きます。  

[OctopressからHugoへ移行した](http://deeeet.com/writing/2014/12/25/hugo/)  
[ブログをOctopressからHugoに移行した](http://yet.unresolved.xyz/blog/2015/01/04/migrate-blog-to-hugo-from-octopress/)  

ブログを書く上で２つの条件がありました。  

 - Markdownで書けること
 - 自分で記事を管理出来ること

条件を満たしているブログ作成ツールは他にもあると思いますが、
あまり悩んでいてもブログを書き始めることが出来ないので、
ひとまずはHugoで始めることにしました。  

Hugo以外の候補としてはOctopressがありましたが、紹介したサイトにある通り、
記事が増えると記事生成の速度に問題があるとのことなので、Hugoを選びました。  

### Hugoのメリット

#### 構造がシンプル

Hugoのファイル構成はシンプルで理解しやすい内容になっています。  
テーマについても比較的、理解しやすくカスタマイズしやすい構造となっています。  

#### 速い

速度面については記事数が少なく、比較対象もないので何とも言えませんが、
遅く感じることは一切ありません。  

### Hugoのデメリット

#### テーマが少ない

選択できるテーマが少ないです。  
私は現在[hyde](https://github.com/spf13/hyde)というテーマを使っていますが、
今後自分でテーマを作成して運用していきたいと思っています。  
テーマについてはこれから増えていくことに期待しましょう。  

### 今後について

Wercker CIを使ってデプロイの自動化を試していこうと思っています。  

[Automated deployments with Wercker](http://gohugo.io/tutorials/automated-deployments/)  
