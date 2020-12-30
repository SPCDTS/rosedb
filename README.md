# rosedb
rosedb 是一个简单、高效的 K-V 数据库，使用 Golang 实现，支持多种数据结构，包含 `String`、`List`、`Hash`、`Set`、`Sorted Set`，接口名称风格和 Redis 类似。

## 为什么会做这个项目

大概半年前（2020 年中），我刚开始学习 Go 语言，由于之前有 Java 语言的经验，加上 Go 的基本语法较简单，上手还是很快，但是学完基础的语法知识之后，就不知道下一步应该做什么了。

我对于数据库还是比较感兴趣的，因此想着可以自己实现一个简单的，造个轮子来玩玩，借此巩固自己的一些基础知识。

因此这个项目也是学习并巩固相关知识的不错的素材，通过实践这个项目，你至少可以学到：

* Golang 大多数基础语法，以及一些高级特性。由于是纯 Golang 实现，因此 Go 语言的基本程序结构、变量常量结构体、常用数据结构如 slice map、单元测试等等都会涉及到；还会有比如高级函数、互斥锁的使用。
* 数据结构。Redis 包含的几种数据结构在这个项目中都有体现，链表，哈希表，数组等一些常用的数据结构要能够写出来，跳表这种稍微困难的数据结构，就算不能直接写出来，也必须能够了解其特点，时间空间复杂度，使用场景等。
* 操作系统。特别是对文件系统，内存映射要有一些了解。

对于抱着学习目的来看这个项目的同学，有一些小小的建议：

这个数据库的模型非常的简单易于理解，后续我会整理成文档分享出来，所以你要相信自己肯定能够看懂，尽管刚开始看的时候可能有点困难。

你需要有一些预备知识，Go 基础语法肯定不用说了，特别是数据结构要有一些了解，不然一些代码可能理解起来比较的困难。

由于个人能力有限，因此欢迎大家提 Issue 和 Pr，一起完善这个项目。

## 安装

项目基于 Go 1.14.4 开发，首先需要确保安装了 Golang 环境，安装请参考 [Golang 官网](https://golang.org/)。

使用 `go get github.com/roseduan/rosedb` 安装，然后在你的项目中 import 即可：

```go
import (
		github.com/roseduan/rosedb
)
```

## 使用

### String

### List

### Hash

### Set

### Sorted Set

## 待办

+ [ ] 支持 TTL
+ [ ] 支持事务，ACID 特性
+ [ ] 数据压缩
+ [ ] String 类型 key 加入前缀扫描
+ [ ] 缓存淘汰策略
+ [ ] 写一个简单的客户端，支持命令行操作
+ [ ] 完善相关文档
