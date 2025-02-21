---
title: 🎉 部署PVE服务器虚拟化管理软件
summary: PVE软件（Proxmox Virtual Environment）是一款开源的虚拟化管理平台，主要用于创建和管理虚拟机（VM）及容器（LXC）
date: 2025-02-10

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com)'

authors:
  - 不白炖

tags:
  - Proxmox VE
  - 服务器运维
  - 虚拟化
---

大家好，我是**不白炖**

今天我要给大家介绍的是如何使用部署PVE服务器虚拟化管理软件

## 背景：

家里最近装修完了，搞了条1000M的宽带，想着能不能搞点什么利用好这个宽带。刚好最近手机储存满了，突然想到为何不做一个NAS呢，经过几天的技术方案筛选，最后决定使用黑群晖作为NAS的管理系统，但是由于黑群晖的系统内核版本较低，所以我打算部署多个系统作为家用方案，所以这里用到了PVE来管理服务器



## 使用到的物料：

### 硬件：

u盘一个、电脑或者服务器一个。我家里用的是汪汪队射手开源的QNSA方案，自己diy了一个6盘位的NAS，CPU采用N100，作为nas足够了，还能进行影片硬解码，播放蓝光影片没问题

### 软件：

pve安装镜像、Rufus USB启动盘制作工具



## 步骤：

1. 制作启动盘

在PVE官网下载好官方的安装镜像后打开Rufus软件，插入U盘，选择U盘，然后选择PVE的镜像，然后点击开始，等待制作完成即可，详情制作启动盘的文章可以参考如何使用Rufus制作启动盘



2. 刷写入镜像

将制作好的启动盘插入NAS的USB口内，插好鼠标和键盘，通电后按F12进入启动菜单键，选着你U盘相对应的名称，开始进入引导，等到一会即可进入安装界面，选择好地区，写入的硬盘，ip地址等信息，点击开始即可完成安装



3. 进入管理页面

默认的管理页面是刚才安装界面设置的IP:8006，默认账号是root，默认密码也是root，输入后就能看到默认界面



以上就是使用U盘安装PVE的教程了，后续我会出一期PVE的具体使用以及汉化，显卡直通等教程

