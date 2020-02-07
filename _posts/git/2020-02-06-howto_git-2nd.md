---
title:  "gitリモートリポジトリとロカールリポジトリの統合"
excerpt: "git fetch、merge、pullについて"

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
  - "2020"

#last_modified_at: 2020-02-06T14:47:00-00:00

---

## git fetch

単純にリモートリポジトリの最新情報をロカールリポジトリに持ってくるだけなら、
```git pull``` コマンドで十分だが、リモートリポジトリの内容を確認して統合したくないとき
```git fetch```を使えられる。

> ```fetch```を実行すると、リモートリポジトリの最新情報を確認できます。
そのときロカールに持ってきたブランチは名前内ブランチで取り込まれる。
このブランチは「FETCH_HEAD」で、チェックアウトすることもできる。

例えば、ロカールとリモートリポジトリのBまで進められた状態で、```fetch```を実行すると
以下のようになる。

![img1](http://drive.google.com/uc?export=view&id=1zw5Ynr0ekLJYPGbraMVylaaqme7mBU8y)

<br>

この状態でリモートリポジトリの内容をロカールの「master」に統合したい場合は「FETCH_HEAD」ブランチを```merge```するか、予め```pull```を実行すればよい。

## git merge

「FETCH_HEAD」ブランチを```merge```すると、ローカルの「master」ブランチに統合される。

![img2](http://drive.google.com/uc?export=view&id=1MpsIjIGbF8hjfHMEgxrOo9U5ueobR7KT)

