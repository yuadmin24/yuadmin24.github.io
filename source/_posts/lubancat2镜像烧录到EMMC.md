---
title: lubancat2镜像烧录到EMMC
categories: [硬件开发]
tags: [配置方法,硬件烧录]
---

lubancat2镜像烧录

<!--more-->

## 1.下载驱动

### 	①打开DriverAssitant_v5.1.1

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/1b5b54255c09261668646.png)

### 	②运行DriverInstall.exe(确保驱动正确安装，先选择执行'驱动卸载'，再执行'驱动安装')

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/e836700bebb52bcf1fbec.png)

## 2.镜像烧录

### 	①进入镜像烧录软件RKDevTool_Release_v2.86

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/2ffc175fcf72a22e0a085.png)

### 	②运行RKDevTool.exe

### 	③将准备好的lubancat2板卡按以下图片提示操作

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/388ab8bddeee1d4cb1bbb.png)

### 	④若识别成功，则会出现'发现一个MASKROM设备'(若未识别成功,回到步骤③,重复执行)PS:若多次未识别成功,可换条数据线重试

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/8109b94f57a994a30465f.png)

## 3.Boot和system的选择

### 	①此板卡为lubancat2,boot选择RK356X的(选择错误，会导致后续烧录镜像失败)

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/7bd424f4d6e51045f67c8.png)

### 	②system为烧录的img镜像文件，若下载的格式为'.img.gz',需解压为'.img'文件(选择为非.img文件，会导致后续烧录镜像失败)

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/307f4f37368d2b8c9aa4f.png)

### 	③选择'强行按地址写'

![](https://0dad3a1b.telegraph-image-5zs.pages.dev/file/ce54a1663d8c701622968.png)

### 	④点击'执行'按钮，稍等片刻，镜像烧录成功(若烧录成功,回到步骤①,重复执行)PS:若未烧录成功，可能是选择的boot,system文件错误；烧录成功后，首次系统启动，插电后需要2-3min初始化