# 一、概述

本文为你介绍了路由器端三段测速CLI的使用方法，帮助你快速集成三段测速服务。

## 前提条件

环境要求如下表所示

| **类别** | **说明** |
| --- | --- |
| 系统版本 | 支持Linux、Windows、macOS |
| 系统位数 | 支持32位和64位 |

## 集成CLI

### 下载CLI

你需要下载相应平台的CLI并放置在合适的文件夹下。

| **文件名称** |
| --- |
| speedtest-cn-node |

### 获取AppId、AppKey和ProductId

AppId、AppKey和ProductId是申请的应用的唯一标识，[点击获取](https://b.speedtest.cn/)。

### CLI参数说明

| 命令 | **说明** | 是否必选 |
| --- | --- | --- |
| -a string | 申请的AppId | 是 |
| -k string | 申请的AppKey | 是 |
| -p string | 申请的ProductId | 是 |
| -d string | 监听地址（默认：0.0.0.0） | 否 |
| --port int | 端口号（默认：51090） | 否 |
| -t int | 线程数（默认：4） | 否 |
| -v | 版本信息 | 否 |
| -h | 帮助文档 | 否 |

### CLI调用方式

```shell
./speedtest-cn-node -a AppId -k AppKey -p ProductId -d 0.0.0.0 --port 51090
```
