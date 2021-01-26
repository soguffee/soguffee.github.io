---
title:  "[security]WAFとは？"
excerpt: "WAF"

toc: true
toc_sticky: true
toc_label: "On this page"
toc_icon: "file-alt"

comments: true
categories:
  - security
tags:
  - Study
  - security
  - "2021"
last_modified_at: 2020-02-18T19:22:00-00:00

---

## WAFとは

### Webアプリケーションを攻撃から守るシステム
WAF(Web Application Firewall)は一般的なFW(Firewall)と違い、ウェブアプリケーションセキュリティを極めた開発されたシステムだ。

### ファイアウォールとの違い
一般的なファイアウォールとWAFの大きな違いは、防御の対象だ。
一般的なファイアウォールが企業や官公庁の内部ネットワークへの不正アクセスを防ぐのに対し、WAFはWebアプリケーションやWebサーバへの不正アクセスを防ぐ。ただし、外部からの攻撃を防ぐ方法が同様であるため、WAFもファイアウォールの一種と考えられるでしょう。

## WAFの概念と原理

### ウェブアプリケーションの理解
WAFを知るためにウェブアプリケーションについて知る必要がある。
ウェブアプリケーションはインタネット上で利用している応用ソフトウェアを意味し、主にOSIモデル7階層に該当する。
ウェブアプリケーションの構造は一般的に以下の図のように表現できる。
<img src="http://drive.google.com/uc?export=view&id=1HXDUl7f4Bys8LgX8V8fdw3RpKJifAkvP" width="80%" height="60%" style="margin-left: auto; margin-right: auto; display: block;"> <br>

## WAFの仕組み
WAFでは「シグネチャ」を用いて不正アクセスを防止する。「シグネチャ」とはアクセスのパターンを定義したもので、このパターンに一致するアクセスがあった場合に、通信許可と拒否の判断を行うという仕組みだ。

WAFの不正アクセス検知方式には「ブラックリスト方式」と「ホワイトリスト方式」の２種類がある。

<img src="http://drive.google.com/uc?export=view&id=1BVstOc2lP3FS_JhVsXssGoAKBaidP79l" width="80%" height="60%" style="margin-left: auto; margin-right: auto; display: block;"> <br>

WAFが設置される場所は、クライアントとWebサイトの間だ。
あくまでもイメージとなるが、「クライアント（ブラウザなど）⇔WAF⇔Webサイト」といった関係にある。
Webアプリケーションを利用するユーザーは、HTTP通信によって情報をやり取りする。ユーザーが書き込みや参照などの操作をすると、要求（リクエスト）がWebサイトに送られ、その結果（レスポンス）をユーザーに返す。このとき、データベースを不正に操作するような通信が紛れていると、情報漏えいなどの事件につながる恐れがある。

そこで、WAFの登場。WAFはHTTP通信の内容を1つ1つ検査することで、不正アクセスがないかを監視する。不正アクセスをブロックし、正規のユーザーからのアクセスは許可するという考え方で、シグネチャによるパターンマッチングを基本とし、シグネチャ以外の機能や独自の検査ロジックを組み合わせることで検査の精度を高めているWAFが多くなっている。
