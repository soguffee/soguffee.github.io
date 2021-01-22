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
