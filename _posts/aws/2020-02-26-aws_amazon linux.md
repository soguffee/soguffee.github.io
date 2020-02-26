---
title:  "AWS Amazon Linux"
excerpt: "現在私が使用しているAWSインスタンスのOSについて"

toc: true
toc_sticky: true
toc_label: "On this page"
toc_icon: "file-alt"

comments: true
categories:
  - aws
tags:
  - Study
  - aws
  - japanese
  - "2020"
last_modified_at: 2020-02-03T16:36:00-00:00

---

AWSで使用しているOSはAmazon Linux AMIです。
Amazon LinuxはCentOSに基盤していて、RedHat Enterprise Linux AS基盤のリナックスリリース版である。

* 参考
[Amazon Linux Reference](http://centos.pe.kr/owiki/index.php?url=centos "Amazon Linux Reference")

<br>

### 本文で抜粋

```
Amazon Linux is provided by Amazon Web Services (AWS). 
It is designed to provide a stable, secure, and 
high-performance execution environment for applications 
running on Amazon EC2. It also includes packages that enable
easy integration with AWS, including launch configuration 
tools and many popular AWS libraries and tools. AWS provides
ongoing security and maintenance updates for all instances
running Amazon Linux. Many applications developed on CentOS
(and similar distributions) run on Amazon Linux.
```

つまり、Amazon Linux AMIはCentOSと交換になる。

## 特徴
> メリット
* マゾンが開発、保守するため、サポート受けやすい
* RedHatベースのため実務で向上したOSだ
* Amazon Web Servicesとの連携が良い
* Amazon独自リポジトリを支援された素早い`yum`

> デメリット
* RebHatやCentOSから利用出来るyumパッケージが投入出来ない場合もある

