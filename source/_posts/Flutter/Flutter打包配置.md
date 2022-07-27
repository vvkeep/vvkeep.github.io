---
title: Flutter 证书和打包配置
date: 2022-07-27 09:03:23
tags:
---


# 一、iOS证书配置

* 1. iOS证书配置网址
  ```
  https://developer.apple.com/account/
  ```

* 2. 添加包名
![01](./Flutter打包配置/01.png)
![02](./Flutter打包配置/02.png)

* 3. 制作证书
![03](./Flutter打包配置/03.png)
![04](./Flutter打包配置/04.png)
![05](./Flutter打包配置/05.png)
![06](./Flutter打包配置/06.png)
![11](./Flutter打包配置/11.png)

* 3. 制作描述文件
![07](./Flutter打包配置/07.png)
![08](./Flutter打包配置/08.png)
![09](./Flutter打包配置/09.png)
![10](./Flutter打包配置/10.png)

# 二、本地真机调试(常见错误)
![100](./Flutter打包配置/100.png)
* 华为二维码扫描库仅支持Arm64架构，Xcode默认支持Arm64和ArmV7，所以在Xcode中移除V7架构
  
![101](./Flutter打包配置/101.png)
* 华为二维码扫描库不支持Bitcode,在Podfile文件中关闭bitcode

![102](./Flutter打包配置/102.png)
* 第一次运行需要安装依赖(pod install)

# 三、配置启动图和AppIcon
* 启动图配置
![105](./Flutter打包配置/105.png)



# 二、iOS/Andorid多环境打包


