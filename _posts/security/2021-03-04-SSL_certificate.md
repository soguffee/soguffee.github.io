---
title:  "[security]SSL認証書の種類"
excerpt: "SSL認証書の種類"

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
last_modified_at: 2021-03-04T01:00:00-00:00

---

## SSLサーバ証明書の種類(認証レベル)

SSLサーバ証明書には大きく分けて
「ドメイン認証（DV: Domain Validation）型SSLサーバ証明書」
「企業認証（OV: Organization Validation）型SSLサーバ証明」
「EV（Extended Validation） SSL証明書」
の3種類があります。
それぞれの証明書でSSLによる通信の暗号化機能の違いはほとんどありませんが、サイトやサイト運営者の実在証明といった機能の面で大きく違いがあります。

<img src="http://drive.google.com/uc?export=view&id=1SN7CXTBmSLE6WhKFx8AHX3GBq1qm_cjh" width="80%" height="60%" style="margin-left: auto; margin-right: auto; display: block;"> <br>

## ドメイン認証（DV: Domain Validation）型SSLサーバ証明書
SSL証明書発行の際に、ドメインの管理者に認証を得てから発行されるSSL証明書です。
ドメインの管理者に認証を得ることでサイト所有のドメインの使用権の有無を認証します。
SSL証明書の中で認証レベルは最も簡易的なものとなりますが、最短で即日から取得可能で、料金を他のSSL証明書と比べ安く取得がしやすい証明書です。
個人の方や安価にSSLを導入されたい方にお勧めのSSL証明書です。

## 企業認証（OV: Organization Validation）型SSLサーバ証明書
ドメインの使用権の有無だけでなく、サイトの運営者（証明書に記載される組織）が実在するかどうか確認した上で発行されるSSL証明書です。
企業・組織の実在性を、登記事項証明書や第三者データベースに基づき確認し、発行の際に電話確認を行うことで組織の法的実在の確認を行います。
個人の方は取得することができません。
認証強度が強く、高い信頼性を実現するSSL証明書です。
クレジットカード番号を盗み取ろうとするフィッシング詐欺への対策としてもご利用いただけますので、サイト内で重要な情報のやり取りを行う方にお勧めのSSL証明書です。

## EV（Extended Validation） SSL証明書
企業認証型SSLよりも、より厳格に実在性の確認を行った上で発行されるSSL証明書です。
CA/Browser Forumのガイドラインに基づき厳格な審査のもと発行されるため、認証レベルが最も高く、金融機関でも多く使われています。
EV SSL証明書が導入されているウェブサイトにアクセスすると、ウェブブラウザのアドレスバーが緑色に変わり、サイト運営団体名が表示されるなど、セキュリティ対策が実施されている安全なサイトであることをサイト利用者にわかりやすく伝えることができます。
認証レベルを高く保ちたい方や、サイトの利用者へ安全性をアピールされたい方にお勧めのSSL証明書です。
