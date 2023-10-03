---
title: Windows7/10/11下Java环境配置
categories: [Java开发]
tags: [环境配置, 配置方法]
---
Java PATH配置

<!--more-->

## 1.下载JDK

​	最新下载地址：https://www.oracle.com/java/technologies/downloads/

​	JDK8下载地址：https://www.oracle.com/java/technologies/downloads/#java8-windows

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/273f7378c5fce617a0cd7.png)

## 2.安装JDK（这里以JDK8为例）

### 	1.准备工作

​		①下载好的jdk-xxxx-windows-x64.exe安装程序

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/52f1a1796b4f0e472b097.png)

​		②在C盘根目录创建文件夹名："java"，以及二级文件夹"jdk"和"jre"

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/d987f772b9371d3c0d1b6.png)

### 	2.安装

​		①以管理员身份运行jdk-xxxx-windows-x64.exe

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/ec2d4c92095ab05293f43.png)

​		②点击下一步

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/85709fff42b922c6c5312.png)

​		③更改为刚刚创建好的java文件夹下的jdk文件夹

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/8c3406c0674f22d00d3e2.png)

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/476e4304044d65dce0df7.png)

​		④点击'"下一步"

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/603950f7e4782be644671.png)

​		⑤等待安装

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/b1ac504121320d4f979d0.png)

​		⑥更改为刚刚创建好的java文件夹下的jre文件夹，点击"下一步"

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/57b87451e11731e15b38d.png)

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/2fc02875486a39900d812.png)

​		⑦等待安装完毕并关闭

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/f3bc5e7e65948f2515888.png)

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/77bfbe1868aa8f048da1c.png)

## 3.配置PATH

​		①打开此电脑设置-关于-高级系统设置

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/850f6c06e5fc290afa0b4.png)

​		②打开"环境变量"

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/d2792c2982013b0e994de.png)

​		③找到下面的"系统变量",点击下方的"新建"

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/db6892b9ec3dd41f7c3c3.png)

​		④输入变量名为JAVA_HOME，变量值为C:\java，点击确定

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/de3f5223620703ad58731.png)

```c
JAVA_HOME
```

```c
C:\java
```

​		⑤找到Path,并双击打开

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/d6109223ffb6990967ada.png)			⑥点击右边导航栏的"新建"

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/b705c1875cd36627ee418.png)			⑦新建两个环境变量

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/5aaa446a77ae9ba666756.png)

```c
%JAVA_HOME%\jdk\bin
```

```c
%JAVA_HOME%\jre\bin
```

​		⑧一直点确定按钮，一直到返回桌面设置

## 4.测试配置是否成功

​		①键盘win+r,输入'CMD'，打开CMD

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/fb6b7d9c8ce4d8b304dad.png)

​		②输入java -version,回车

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/d0a2348a142beee9124f1.png)

```shell
java -version
```

​		配置成功反应：

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/d4994383875d3bf182c6a.png)

​		③输入javac -version

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/3605878cf6e59484fbbc5.png)

```shell
javac -version
```

​		配置成功反应：

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/9ea096157a8a3bcadc0cf.png)

## 5.第一个Java程序

​		①程序

```java
public class helloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

​		②输出

```shell
Hello World!
```
