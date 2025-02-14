---
layout: default
title: DNS Reconnaisance
description: Information Gathering Materials
---

## Introduction

Sebelum memulai lab, baik untuk dibahas terlebih dahulu tentang apa itu DNS?

```
USER: saya mau mengunjungin google.com, IP address nya apa?
    DNS: google.com -> 8.8.8.8 
USER: IP address 8.8.8.8 itu milik siapa yah?
    DNS: 8.8.8.8 -> google.com
```

1.  DNS adalah kepanjangan dari Domain Name System.

2.  Bertugas untuk melakukan pemetaan dari IP address ke sebuah nama domain atau kebalikannya.

Berikut adalah struktur format dari nama DNS([ref](https://www.jogjahost.co.id/blog/dns-server-adalah/)):

![DNS_STRUCTURE](/assets/subdomain.webp)

### Apakah nama-nama domain ini perlu kita cari tahu sewaktu melakukan project _penetration testing_?

Jawaban:
Tergantung dari permintaan klien! tetapi dari kebanyakan kasus, anda tidak perlu melakukannya.

Kenapa?
Penetration Testing secara dasar sangat berfokus pada cangkupan jadi jika klien hanya mencantumkan target website "website-test.id", berarti yang di uji keamanannya hanya di domain itu saja. Anda tidak perlu mencari subdomain atau domain yang lain.

Jadi kapan pakai teknik ini?
1.  Lakukanlah jika anda melakukan _bug bounty_ karena tipikal nya secara umum program ini mencakup banyak aset yang harus di uji oleh _bug hunter_, jadi dengan melakukan DNS reconnaisance/enumeration _bug hunter_ bisa memilah dan memetakan aset yang dapat dia uji sesuai dengan prosedur dari programnya.
2.  Lakukanlah jika anda mau melakukan pemetaan aset eksternal perusahaan kalian. Dengan melakukan DNS reconnaisance/enumeration anda bisa melihat aset-aset eksternal website anda yang dapat dijadikan sasaran oleh penyerang siber. Dengan pendekatan ini anda bisa menaruh prioritas mana aset digital anda yang terlebih dahulu mesti diamankan.

## Lab

Untuk melakukan DNS reconnaisance/enumeration sendiri anda dapat memanfaatkan program dari _3rd party_ ini:

1.  [crt.sh](https://crt.sh/)

2.  [c99](https://subdomainfinder.c99.nl/)


