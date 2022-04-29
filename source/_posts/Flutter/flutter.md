---
title: flutter
date: 2022-04-24 19:04:00
tags:
---

Flutter 打包 NoSuchAlgorithmException: Algorithm HmacPBESHA256 not available
在这句话后面添加 -storetype jks就可以了
keytool -genkey -v -keystore ~/打包的名字.jks -keyalg RSA -keysize 2048 -validity 10000 -alias key -storetype jks 
