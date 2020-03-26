---
title:  "[Linux]nohup"
excerpt: "リナックスコマンドnohupと'&'について"

toc: true
toc_sticky: true
toc_label: "On this page"
toc_icon: "file-alt"

comments: true
categories:
  - linux
tags:
  - Study
  - linux
  - japanese
  - "2020"
last_modified_at: 2020-02-18T19:22:00-00:00

---

## nohup

* Linux、Unixシェルスクリプト(`*.sh`)をdeamon形態で実行するプログラム
* セッションが切れても止まらず動作させる。
* なお、nohupコマンドで実行されたスクリプトの標準出力及び標準エラー出力はプログラムを実行しているディレクトリにnohup.outというファイル名で保存されます。ディレクトリに書き込み権限がなければ$HOME/nohup.outとして保存される。

## &

* プロセス実行の際バックグラウンドで実施させるコマンド
* セッションが切れたら止まってしまう。

### 使い方

以下のように`nohup`コマンドを使い、かつ`&`の指定によってシェルスクリプトをバックグラウンドで動かせば良い

```
$nohup ./batch.sh &
```

### 終了方法

killコマンド私用

```
$kill -9 PID
```

*参考
