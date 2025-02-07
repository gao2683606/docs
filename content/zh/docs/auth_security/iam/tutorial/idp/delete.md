---
title: "删除认证源"
date: 2021-12-07T11:35:50+08:00
weight: 90
description: >
    删除认证源
---

该功能用于删除认证源。

{{% alert title="注意" color="warning" %}}
- SQL认证协议的认证源不支持删除。
- 当认证源不支持自动创建用户，作为辅助认证源使用时，只要认证源禁用即可删除。
- 当认证源支持自动创建用户，分为两种情况：
    - 用户归属域为系统已有域时，只要认证源禁用即可删除认证源及认证源下的用户和组。
    - 用户归属域为空即自动创建域时，需要认证源自动创建的域下没有项目，且认证源禁用才可以删除认证源即认证源自动创建的域、用户、组。
{{% /alert %}}

**单个删除**

1. 在认证源页面， 单击"禁用"状态的认证源右侧操作列 **_"删除"_** 按钮，弹出操作确认对话框。
1. 单击 **_"确定"_** 按钮，完成操作。

**批量删除**

1. 在认证源列表中勾选一个或多个认证源，单击列表上方的 **_"批量操作"_** 按钮，选择下拉菜单 **_"删除"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。