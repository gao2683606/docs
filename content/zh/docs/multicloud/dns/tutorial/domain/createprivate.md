---
title: "新建PrivateZone域名"
date: 2021-11-25T15:16:18+08:00
weight: 20
description: >
    新建PrivateZone类型的域名并将其同步到公有云
---

PrivateZone域名是基于VPC网络的私有DNS服务，支持使用私有域名来解析VPC环境中的资源，私有域名在VPC外无法访问。

**使用流程**

- 新建PrivateZone域名。
- 在域名详情-记录中添加记录。
- 通过关联VPC功能将PrivateZone域名同步到公有云。目前支持平台：阿里云、AWS。

### 新建PrivateZone域名

该功能用于新建PrivateZone域名。

1. 在DNS解析页面，单击列表上方 **_"新建"_** 按钮，弹出新建域名对话框。
2. 配置以下参数：
   - 指定域：选择DNS解析所属的域。
   - 解析域类型：选择PrivateZone域名。
   - 域名：设置需要解析的域名。其中PublicZone类型目前仅支持二级域名。
3. 单击 **_"确定"_** 按钮，进入同步到公有云页面。
4. 如需要将域名同步到公有云，则需要选择区域以及对应的VPC，配置完成后，单击 **_"确定"_** 按钮。
5. 如暂不需要将域名同步到公有云，则直接单击 **_"跳过"_** 按钮即可。


### 关联VPC

该功能用于将PrivateZone类型的解析域名关联到VPC，关联VPC的同时还会将域名同步到对应公有云平台。

{{% alert title="说明" %}}
腾讯云不支持PrivateZone类型的DNS，即不能关联腾讯云的VPC。
{{% /alert %}}

1. 在DNS解析页面，单击域名右侧操作列 **_"关联VPC"_** 按钮，弹出关联VPC对话框。
2. 设置以下参数：
   - 区域：设置区域，并通过区域过滤VPC。可通过城市、平台快速过滤筛选出合适区域。
   - VPC：选择要关联的VPC，关联后将会把DNS解析域名同步到VPC所在平台账号中。
3. 单击 **_"确定"_** 按钮，完成操作。 