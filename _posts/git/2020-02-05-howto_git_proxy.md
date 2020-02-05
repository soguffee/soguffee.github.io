---
title:  "プロキシ環境でgitへ接続"
excerpt: "プロキシ環境でgitを使うために"

#toc: true
#toc_sticky: true
#toc_label: "On this page"
#toc_icon: "file-alt" 

comments: true
categories:
  - git
tags:
  - Study
  - Git
  - japanese
  - "2020"
last_modified_at: 2020-02-05T17:19:00-00:00

---

# gitがプロキシサーバーと動作させる

## プロキシ設定を確認
```
> git config --global --get http.proxy
```

## プロキシ設定する
```
> git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080
```

```proxyuser``` ：プロキシユーザー  
```proxypwd``` ：プロキシパスワード  
```proxy.server.com``` ：プロキシサーバーのURL  
```8080``` ：プロキシサーバーのポート  


## プロキシ設定を解除
```
> git config --global --unset http.proxy
```
