---
title: "密码策略"
date: 2022-01-20T19:33:48+08:00
weight: 30
description: >
    用于配置密码复杂度、有效期等信息
---

密码复杂度、有效期等配置信息仅针对本地SQL用户生效。


1. 在左侧导航栏，选择 **_"系统配置/全局设置/全局设置"_** 菜单项，进入全局设置页面。
2. 支持配置以下信息：
    - 密码不重复次数：用户密码最近n次不能重复。即新设置的密码不能和最近n次的密码重复。例如：若设置为3，则新密码不能与之前3次已使用过的历史密码相同。默认为空，代表没有限制。仅适用于本地SQL用户修改密码。
    - 密码最小长度：限制用户密码的最小长度，新建用户或重置密码时，密码长度必须符合要求。默认为6位。仅适用于本地SQL用户修改密码。
    - 密码不重复次数：用户密码最近n次不能重复。即新设置的密码不能和最近n次的 密码重复。例如：若设置为3，则新密码不能与之前3次已使用过的历史密码相同。默认为空，代表没有限制。仅针对本地SQL用户有效。
    - 密码最小长度：限制用户密码的最小长度，新建用户或重置密码时，密码长度必须符合要求。默认为6位。仅针对本地SQL用户有效。
    - 连续登录失败次数：设置用户连续登录失败的次数上限，当连续登录失败次数超过设定值，账户将会被锁定，需要管理员启用用户并重置密码。默认值为空，代表没有限制。仅针对本地SQL用户有效。
    - 密码有效期：设置用户默认密码有效期，0代表无限制。仅针对本地SQL用户有效。
    - 用户密码复杂度：设置用户密码的复杂度，可以限制密码必须包含大写字母、小写字母、数字或符号中的任意N种，1代表无限制，4代表需要密码包含以上4种。仅适用于本地SQL用户修改密码。