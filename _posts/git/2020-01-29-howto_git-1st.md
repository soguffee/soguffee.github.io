---
title:  "git使い方メモ"
excerpt: "gitの使い方を気軽く見てみよう"

toc: true
toc_sticky: true
toc_label: "On this page"
toc_icon: "file-alt"

comments: true
categories:
  - git
tags:
  - Study
  - Git
  - japanese
  - 2020
last_modified_at: 2020-01-29T16:30:00-00:00

---

# git使い方

## 1. はじめに
### 1.1 OS
* Windows10

### 1.2 インストール
[Git for Windows](https://gitforwindows.org/)

## 2. リポジトリの設定

### 2.1 ローカルリポジトリを作成する
```
> git init
```
* ```git init ```でカレントフォルダを Git のリポジトリにできる。

### 2.2 リモートリポジトリに接続させる

* 繋がっているリモートリポジトリを確認

```
> git remote -v
```
<br>

* リモートリポジトリを追加する

```
> git remote add origin <url>
```
<br>

* リモートリポジトリから削除する

```
> git remote remove origin
```
<br>

### 2.3 リポジトリをクローンする
```
git clone <リポジトリフォルダへのパス>
```
カレントフォルダにリポジトリと同じ名前のフォルダが作成され、そこがクローンしたリポジトリ兼作業ディレクトリになる。

## 3. コミット時のユーザー名・メールアドレスを設定する

```
> git config --global user.name <ユーザー名>

> git config --global user.email <メールアドレス>
```

```git config``` で Git の設定をできる。  
```user.name``` がコミット時のユーザー名、 ```user.email``` がメールアドレスの設定。  
```--global``` オプションをつけると、現在のユーザー（OS）で Git を使った場合のデフォルト値を設定できる。  
```--global``` を省略した場合は、現在のリポジトリだけで有効な設定になる。  

## 4. ステージング

![Alt text](..\..\image\1_contents_2020-01-29-howto_git-1st_1.jpeg)

<br>

Git では、コミットしたい変更内容を一旦「ステージング」と呼ばれる領域に登録する。
そしてコミットをすると、ステージングに登録されていた変更内容だけがリポジトリに反映される。

```add``` コマンドは、このステージングに変更内容を登録する。

ステージングが存在することで、１つのコミットに含める変更内容をファイル単位で細かく制御できるようになる。  

### 4.1 ファイルをステージングに追加する

```
> git add <ファイル or フォルダ>
```
<br>

**\<Tip\>**

```
> git add -p
```
ステージングと同時に変更履歴を確認出来る。


### 4.2 ステージングに登録した内容を取り消す
```
> git reset
```

