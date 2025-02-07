---
title: "创建私有云IP子网"
date: 2022-01-04T15:30:18+08:00
weight: 10
description: >
    创建私有云平台IP子网
---

请确保已添加对应私有云平台的云账号。

1. 在IP子网页面，单击顶部“私有云”页签，单击列表上方 **_"新建"_** 按钮，进入新建私有云的IP子网页面。
2. 设置以下信息：
    - 指定项目：选择IP子网的所属项目。
    - 区域：选择IP子网所属区域。
        - 当区域选择为“OpenStack”的区域时：
            - VPC：选择OpenStack平台上的VPC。
            - 可用区：设置IP子网所属的可用区。一个VPC下可以有多个可用区的IP子网，同一VPC下不同可用区的子网默认互通。
        - 当区域选择为”ZStack/DStack“的区域
            - VPC：选择ZStack/DStack平台上的二层网络。
            - 二层网络：设置IP子网所属的二层网络。
    - 名称：设置IP子网的名称。
    - 子网网段：设置IP地址范围段，格式如192.168.0.0/24，IP子网需要在VPC的网段范围内。
    - 自动调度：启用后，用户创建虚拟机网络指定自动分配时，将从启用自动调度的IP子网中为虚拟机分配IP地址。
3. 单击 **_"确定"_** 按钮，完成创建。