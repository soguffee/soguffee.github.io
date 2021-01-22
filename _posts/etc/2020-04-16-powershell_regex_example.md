---
title:  "括弧()の中の文字だけ読み込む"
excerpt: ""

categories:
  - etc
tags:
  - Study
  - japanese
  - "2020"
last_modified_at: 2020-04-16T17:00:00-00:00
---

# データの整理
実務でデータを成型して括弧()の中の文字だけを読み込む必要があった。
色んな方法があると思うが正規表現(Regex)を利用した方法を紹介する。

```
powershell script .ps1

$ [regex]::maches([対象データ], "\(([^)]*)\)").Groups[1].Value

```

上のような方法で括弧の中の文字列を持ってくることが出来る。
正規表現を覚えとけばこういう時役に立つことが多いと思う。