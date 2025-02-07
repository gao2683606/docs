---
title: "查看节点详情"
date: 2021-12-22T14:57:46+08:00
weight: 70
description: >
    查看负载均衡节点的配置信息
---

1. 在负载均衡节点页面，单击节点名称项，进入节点详情页面。
2. 详情页面顶部菜单项支持对节点进行管理操作。
3. 查看以下信息。
    - 基础信息：查看节点的云上ID、ID、名称、状态、域、项目、集群、主备、上一次心跳、可用区、心跳超时时间、部署机器、创建时间、更新时间、备注。
    - 同步时间戳：表示数据库中负载均衡实例、监听、后端服务器组、后端服务器、转发策略、访问控制、证书等参数在某个特定时间之前已经存在、完整的、可验证的数据写入部署机器。
    - VRRP转发实例配置信息：包括通告间隔、网口、密码、抢占模式、优先级以及路由ID信息。
    - HAProxy配置信息：查看HAProxy配置信息，包括线程数、开启日志、开启HTTP日志、开启Normal日志、开启TCP日志、以及配置模板信息。
    - Telegraf（数据采集工具）配置信息：查看Telegraf配置信息，包括HAProxy上报间隔、数据库名称、地址、以及配置模板信息。
    - KeepAlived配置信息：查看KeepAlived配置模板信息。