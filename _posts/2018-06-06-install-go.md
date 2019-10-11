---
layout: article
author: bing0ne
date: "2018-06-06T15:53:26+08:00"
slug: "install-go"
title: "使用Homebrew安装配置golang环境"
tags: 
    - GO
    - ENV

description: "Go 语言是一个将静态语言的安全性和高效性与动态语言的易开发性进行有机结合的语言。本文将要介绍如何在OS X通过Homebrew中安装和配置GO。"
categories: ["Dev"]
---

Go 语言是一个将静态语言的安全性和高效性与动态语言的易开发性进行有机结合的语言。<!--more--> 

Go 语言是一门类型安全和内存安全的编程语言。虽然 Go 语言中仍有指针的存在，但并不允许进行指针运算。Go语言有时候被描述为“C类似语言”，或者是“21世纪的C语言”。Go从C语言继承了相似的表达式语法、控制流结构、基础数据类型、调用参数传值、指针等很多思想，还有C语言一直所看中的编译后机器码的运行效率以及和现有操作系统的无缝适配。

## 安装golang

```zsh
$ brew update && brew upgrage
$ brew install go
```


## PATH配置
根据 `brew info go` ,我们发现默认的`gopath`指定在`Users/youname/go`下面，这样很不美观。所以我们为`gopath`指定一个新的地址。

```zsh
$ cd ~
$ vim ~/.zshrc
```

编辑`.zshrc`文件并保存，加入一下内容：

```zsh 
# GO PATH
export GOROOT=/usr/local/opt/go/libexec
export GOPATH=/Users/yourname/Dev/go/go_path
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
```

运行`source .zshrc`使得配置文件得以生效

## 安装GO工具包
这里我们使用了取巧的方式，使用VS CODE的GO插件，自动安装GO需要的工具包。
![](https://o20f5n104.qnssl.com/6-6-2018,-3:56:28-PM.png?imageslim)


