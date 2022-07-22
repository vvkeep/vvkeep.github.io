---
title: MYSQL学习记录
date: 2022-07-18 18:15:46
tags:
---

# 一、时区更改
```
// 查看数据库当前时区信息
SHOW VARIABLES LIKE "%zone%" 

// 查看数据库当前时间
SELECT NOW();

// 设置数据库时区
set time_zone = '+0:00'
```
