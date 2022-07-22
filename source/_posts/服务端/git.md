---
title: git删除本地所有未提交的更改
date: 2022-07-18 18:15:46
tags:
---

1.git
删除本地所有未提交的更改
git checkout . && git clean -xdf

一般 git clean都是配合git reset 使用的

如果你有的修改已经加入了暂存区
那么，命令
git reset --hard
git clean -xdf

git回滚到某一个版本

git reset --hard a136c6923d882ffc9065439f33412936902a1f5d

强制提交：

git push -f origin master

未push但commit回退
1.git reset --soft HEAD^
会保留代码
2.git reset --hard HEAD^
不会保留未提交的代码，回退到上个版本
