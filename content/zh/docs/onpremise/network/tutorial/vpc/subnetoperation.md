---
title: "IP子网其他操作"
weight: 40
description: >
  介绍IP子网的常用操作。
---

## 调整调度标签

该功能用于为IP子网绑定调度标签，绑定调度标签的IP子网将遵循调度策略为虚拟机分配IP地址。

1. 单击IP子网右侧操作列 **_"调整调度标签"_** 按钮，弹出调整调度标签对话框。
2. 选择调度标签，单击 **_"确定"_** 按钮。

## 更改项目

该功能用于更改IP子网所属项目。当IP子网为私有状态时，才可以更改项目。

**单个IP子网更改项目**

1. 在IP子网页面，单击IP子网右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"更改项目"_** 菜单项，弹出更改项目对话框。
2. 修改域和项目，单击 **_"确定"_** 按钮。

**批量更改项目**

1. 在IP子网列表中选择一个或多个IP子网，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"更改项目"_** 菜单项，弹出更改项目对话框。
2. 修改域和项目，单击 **_"确定"_** 按钮。

## 设置共享

该功能用于设置IP子网的共享状态。

项目资源的共享范围有五种：

- 不共享（私有）：即项目资源只能本项目的用户可以使用。
- 项目共享-部分（本域内多项目共享）：即项目资源可以共享到同域下的指定项目（一个或多个），只有本项目和被共享项目下的用户可以使用项目资源。
- 项目共享-全部（本域共享）：即项目资源可以共享给域下所有项目，即项目所在域的用户都可以使用项目资源。
- 域共享-部分（多域共享）：即项目资源可以共享到指定域（一个或多个），只有项目资源所在域和共享域下的用户可以使用项目资源。
- 域共享-全部（全局共享）：即项目资源可以共享给全部域使用，即系统中所有用户都可以使用项目资源。

{{% alert title="说明" %}}
设置域共享的条件：

- 在{{<oem_name>}}平台已开启三级权限。
- 用户处于管理后台。

设置项目共享的条件：

- 用户处于管理后台或域管理后台。

{{% /alert %}}

{{% alert title="注意" color="warning" %}}
- 物理机、PXE、IPMI类型的IP子网建议不要设置为共享状态。
- 本地IDC的IP子网共享范围任意。
- 私有云和公有云的IP子网的共享范围与云账号的共享范围有关。
    - 当云账号不共享时，通过云账号同步下来的资源也不能共享。
    - 当云账号启用共享时，通过云账号同步下来的资源也将随着云账号启用共享。
    - 当云账号启用共享时，通过云账号同步下来的资源可以更改共享范围，请确保共享范围在云账号的共享范围内。
    - 当云账号修改共享范围时，通过云账号同步下来的资源的共享范围要始终保持在云账号的共享范围内。如云账号共享A、B、C、D域，域资源共享A、C域，云账号修改共享范围为A、B域，则域资源只能共享到A域。
    - 云账号共享云订阅时，通过云账号同步下来的域资源不能共享。
{{% /alert %}}


**单个IP子网设置共享**

1. 在IP子网页面，单击IP子网右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"设置共享"_** 菜单项，弹出设置共享对话框。
2. 配置以下参数。
   - 当共享范围选择为“不共享”时，即项目资源的共享范围为私有，仅本项目的用户可以使用。
   - 当共享范围选择为“项目共享”时，需要选择本域下可共享的项目。
       - 当项目选择同域下的一个或多个项目时，即项目资源的共享范围为项目共享-部分，只有项目资源所在项目和共享项目下的用户可以使用项目资源。
       - 当项目选择全部时，即项目资源的共享范围为项目共享-全部，项目所在域下的用户都可以使用项目资源。
   - 当共享范围选择为“域共享”时，需要选择共享的域。
       - 当域选择其中的一个或多个域时，即项目资源的共享范围为域共享-部分，只有项目资源所在域和共享域下的用户可以使用域资源。
       - 当域选择全部时，即项目资源的共享范围为域共享-全部，系统中的所有用户都可以使用项目资源。
3. 单击 **_"确定"_** 按钮，完成操作。

**批量设置共享**

多个IP子网批量设置的共享范围必须相同。否则请单独为IP子网设置共享。

1. 在IP子网列表中选择一个或多个IP子网，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"设置共享"_** 菜单项，弹出设置共享对话框。
2. 配置以下参数。
   - 当共享范围选择为“不共享”时，即项目资源的共享范围为私有，仅本项目的用户可以使用。
   - 当共享范围选择为“项目共享”时，需要选择本域下可共享的项目。
       - 当项目选择同域下的一个或多个项目时，即项目资源的共享范围为项目共享-部分，只有项目资源所在项目和共享项目下的用户可以使用项目资源。
       - 当项目选择全部时，即项目资源的共享范围为项目共享-全部，项目所在域下的用户都可以使用项目资源。
   - 当共享范围选择为“域共享”时，需要选择共享的域。
       - 当域选择其中的一个或多个域时，即项目资源的共享范围为域共享-部分，只有项目资源所在域和共享域下的用户可以使用域资源。
       - 当域选择全部时，即项目资源的共享范围为域共享-全部，系统中的所有用户都可以使用项目资源。
3. 单击 **_"确定"_** 按钮，完成操作。

## 设置自动调度

该功能用于为IP子网启用或禁用自动调度功能，启用后，用户创建虚拟机时网络自动调度时，将从启用自动调度的IP子网中为虚拟机分配IP地址。

{{% alert title="注意" color="warning" %}}
仅虚拟机类型的IP子网支持设置自动调度。
{{% /alert %}}

**单个IP子网设置自动调度**

1. 单击IP子网右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"设置自动调度"_** 菜单项，弹出设置自动调度对话框。
2. 设置是否启用自动调度功能，设置完成后，单击 **_"确定"_** 按钮。

**批量设置自动调度**

1. 在IP子网列表中选择一个或多个IP子网，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"设置自动调度"_** 菜单项，弹出设置自动调度对话框。
2. 设置是否启用自动调度功能，设置完成后，单击 **_"确定"_** 按钮。

## 同步状态

该功能用于获取IP子网的当前状态。

**单个同步状态**

1. 单击IP子网右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"同步状态"_** 菜单项，同步IP子网状态。

**批量同步状态**

1. 在IP子网列表中选择一个或多个IP子网，单击IP子网右侧操作列 **_"批量操作"_** 按钮，选择下拉菜单 **_"同步状态"_** 菜单项，批量同步状态。

## 删除IP子网

该功能用于删除IP子网。已分配IP的IP子网不支持删除。

**单个删除**

1. 单击IP子网右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"删除"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。

**批量删除**

1. 在IP子网列表中选择一个或多个IP子网，单击IP子网右侧操作列 **_"批量操作"_** 按钮，选择下拉菜单 **_"删除"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。


## 预留IP

该功能用于查看IP子网中的预留IP详情，支持新建和释放预留IP。

1. 在IP子网页面，单击IP子网名称项，进入IP子网详情页面。
2. 在IP子网详情页面，单击“预留IP”页签，进入预留IP页面。
3. 查看IP子网中预留IP的信息。

### 新建预留IP

该功能用于新建预留IP，预留IP将不会被云管平台分配给服务器使用。

1. 在预留IP页面，单击列表上方 **_"新建"_** 按钮，弹出新建对话框。
2. 输入IP子网中的需要预留的IP地址(支持一次添加6个IP地址)、预留原因，单击 **_"确定"_** 按钮。

### 释放预留IP

该功能用于释放预留的IP，使其可以被云管平台分配。支持单个或批量释放IP地址。

**单个释放**

1. 在预留IP页面，单击IP右侧操作列 **_"释放"_** 按钮，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。

**批量释放**

1. 在预留IP列表选择一个或多个IP地址，单击列表上方 **_"释放"_** 按钮，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。