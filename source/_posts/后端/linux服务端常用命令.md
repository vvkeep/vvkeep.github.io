---
title: linux服务端常用命令
date: 2022-04-25 22:42:31
tags:
hide: true
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
tar -zcvf spring.log.2022-04-20.12 spring.log.2022-04-20.12.tar.gz

```

```

grep -C 5 foo file 显示file文件里匹配foo字串那行以及上下5行

grep -B 5 foo file 显示foo及前5行

grep -A 5 foo file 显示foo及后5行

首次出现位置
取出文件中关键字keyword 首次出现的前2行
grep  -A10  "keyword" /etc/man.config | head -2


最近一次出现的位置
取出文件中关键字keyword 最近出现的前2行
grep  -B10  "keyword" /etc/man.config | tail -2

```

