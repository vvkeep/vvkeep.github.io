---
title: Socket编程基础
date: 2022-03-05 16:42:37
toc: true
categories: "计算机网络原理"
tags: [网络, Socket]
---

![socket](/img/posts/socket.png)

## 一、套接字与端口号

* 套接字(Socket)：典型的网络应用编程接口
* 端口号：标识套接字
* 扩展常见的端口号
  
    | 端口号               | 描述                     |
    |:-------------------:|:-----------------------:|
    | 20(数据)、21（控制）  | FTP文件传输协议           | 
    | 25                  | SMTP简单邮件传输协议       | 
    | 53                  | DNS域名服务器             | 
    | 80                  | HTTP超文本传输协议        | 
    | 110                 | POP3第三版邮局协议        | 


## 二、Socket API

### 1.创建套接字

```
socket()
```

* 传输层使用UDP协议，创建数据报类型套接字(SOCK_DGRAM)
* 传输层使用TCP协议，创建流式套接字(SOCK_STREAM)
* 应用层数据没有经过传输层，直接到网络层，创建原始套接字(SOCK_RAW)

### 2.Socket API 函数

1.创建套接字：`socket()`

2.绑定套接字的本地端点地址：`bind()`

3.设置监听：`listen()`

4.建立连接

  - TCP客户端：`connect()`
  - TCP服务端：`accept()`

5.接收数据

  - TCP：`recv()`
  - UDP：`recvfrom()`

6.发送数据

  - TCP：`send()`
  - UDP： `sendto()`

7.关闭套接字：`close()`



