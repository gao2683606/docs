---
title: "解绑VPC"
date: 2021-11-25T18:35:23+08:00
weight: 20
description: >
    解除PrivateZone类型域名与VPC的绑定关系
---

该功能用于解除域名与VPC的绑定，解绑后将同步删除缓存记录及公有云平台对应的解析域名等。

**单个解绑**

1. 在DNS解析页面，单击“PrivateZone”类型的域名名称项，进入DNS解析详情页面。
2. 单击“关联VPC”页签，进入关联VPC页面。
3. 单击VPC右侧操作列 **_"解绑"_** 按钮，弹出操作确认对话框。
4. 单击 **_"确定"_** 按钮，完成操作。

**批量解绑**

1. 在DNS解析页面，单击“PrivateZone”类型的域名名称项，进入DNS解析详情页面。
2. 单击“关联VPC”页签，进入关联VPC页面。
3. 在VPC列表中选择一个或多个VPC，单击列表上方 **_"解绑"_** 按钮，弹出操作确认对话框。
4. 单击 **_"确定"_** 按钮，完成操作。


```
# 解绑VPC
$ climc dns-zone-remove-vpcs <DNS解析域名ID或名称> <VPC_IDS>
```