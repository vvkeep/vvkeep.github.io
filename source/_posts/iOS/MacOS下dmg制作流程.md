---
title: MacOS下dmg制作流程
date: 2022-05-10 09:59:42
categories: "iOS"
tags: [MacOS, dmg]
index_img: /images/posts/iOS-MacOS下dmg制作流程.png
---

## 一、归档Release包
1. 菜单栏选择 product -> Archive
2. 点击 Distribute App 按钮，选择 Copy App
   {% asset_img 01.png 600 DistributeApp %}
   {% asset_img 02.png 600 CopyApp %}

3. 点击 Next，选择导出名称和目录, Export 发布包

## 二、制作dmg镜像
1. 新建空白文件夹，重命名文件夹为应用名称，拖入刚导出的应用程序
2. 打开终端命令，进入刚创建文件夹，制作 Applications快捷方式
   ```
   cd /Users/mac/Desktop/JSONConverter 
   ln -s /Applications Applications  
   ```
   {% asset_img 04.png 600 Applications %}

3. 打开磁盘工具 -> 新建映像 -> 基于文件夹新建映像，选择刚创建的文件夹，点击 存储
    {% asset_img 03.png 600 export %}



