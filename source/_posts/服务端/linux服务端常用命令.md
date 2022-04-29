---
title: linux服务端常用命令
date: 2022-04-25 22:42:31
tags:
---

```
tail -f -n200 | grep '全量同步linkedMall商品类别数据结束' spring.log
```

解压某个或多个文件
```
gunzip -v spring.log.2022-04-20.*.gz
```

压缩某个文件
```
tar -zcvf spring.log.2022-04-20.12.tar.gz spring.log.2022-04-20.12

```