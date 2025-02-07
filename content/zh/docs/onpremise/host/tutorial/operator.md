---
title: "宿主机操作"
weight: 5
description: >
 介绍宿主机的常用操作。
---

## 界面操作

### 远程终端

该功能支持ssh远程连接到宿主机。连接之后需要使用初始账号列中的用户名和密码进行登录。

1. 单击指定宿主机右侧操作列 **_"远程终端"_** 按钮，选择下拉菜单 **_"SSH IP地址"_** 菜单项，与宿主机建立web SSH连接。
2. 若宿主机上的22端口被其他应用占用，ssh服务端口为其他端口时，可选择下拉菜单 **_"SSH IP地址:自定义端口"_** 菜单项，在弹出的对话框框中设置ssh服务实际端口号，单击 **_"确定"_** 按钮与宿主机建立web SSH连接。

### 启用

该功能用于启用"禁用"状态的宿主机。启用状态的宿主机用于创建虚拟机。

**单个启用**

1. 在宿主机页面，单击"禁用"状态的宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"启用"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，启用宿主机。

**批量启用**

1. 在宿主机列表中勾选一个或多个"禁用"状态的宿主机，单击列表上方 **_"启用"_** 按钮，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，启用宿主机。

### 禁用

该功能用于禁用”启用“状态的宿主机，禁用状态的宿主机不能创建虚拟机。

**单个禁用**

1. 在宿主机页面，单击”启用“状态的宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"禁用"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，禁用宿主机。

**批量禁用**

1. 在宿主机列表中勾选一个或多个"启用"状态的宿主机，单击列表上方 **_"禁用"_** 按钮，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，禁用宿主机。

### 更改域

该功能用于更改宿主机的所属域。服务器安装自研host服务后将自动上报注册到{{<oem_name>}}平台。自动上报到{{<oem_name>}}平台的宿主机默认都属于default域，用户可通过更改域功能，更改宿主机的所属域。

{{% alert title="说明" %}}
更改域的条件：需同时满足

- 当前用户在管理后台。
- 在{{<oem_name>}}已开启三级权限。
- 宿主机的共享范围为私有。
{{% /alert %}}

**单个宿主机更改域**

1. 在宿主机页面，单击宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"更改域"_** 菜单项，弹出更改域对话框。
2. 选择宿主机所属的域，单击 **_"确定"_** 按钮。

**批量更改域**

1. 在宿主机列表中勾选一个或多个宿主机，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"更改域"_** 菜单项，弹出更改域对话框。
2. 选择宿主机所属的域，单击 **_"确定"_** 按钮。


### 设置共享

该功能用于设置宿主机的共享范围。

域资源的共享范围有三种：

- 不共享（私有）：即域资源只能本域的用户可以使用。
- 域共享-部分（多域共享）：即域资源可以共享到指定域（一个或多个），只有域资源所在域和共享域下的用户可以使用域资源。
- 域共享-全部（全局共享）：即域资源可以共享给全部域使用，即系统中所有用户都可以使用域资源。

{{% alert title="说明" %}}
设置共享的条件：需同时满足

- 当前用户在管理后台。
- 在{{<oem_name>}}已开启三级权限。
{{% /alert %}}

**单个宿主机设置共享**

1. 在宿主机页面，单击宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"设置共享"_** 菜单项，弹出设置共享对话框。
2. 配置以下参数：
   - 当共享范围选择为“不共享”时，即域资源的共享范围为私有，仅本域的用户可以使用。
   - 当共享范围选择为“域共享”时，需要选择共享的域。
       - 当域选择其中的一个或多个域时，即域资源的共享范围为域共享-部分，只有域资源所在域和共享域下的用户可以使用域资源。
       - 当域选择全部时，即域资源的共享范围为域共享-全部，系统中的所有用户都可以使用域资源。
3. 单击 **_"确定"_** 按钮，完成操作。

**批量设置共享**

1. 在宿主机列表中选择一个或多个宿主机，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"设置共享"_** 菜单项，弹出设置共享对话框。
2. 配置以下参数：
   - 当共享范围选择为“不共享”时，即域资源的共享范围为私有，仅本域的用户可以使用。
   - 当共享范围选择为“域共享”时，需要选择共享的域。
       - 当域选择其中的一个或多个域时，即域资源的共享范围为域共享-部分，只有域资源所在域和共享域下的用户可以使用域资源。
       - 当域选择全部时，即域资源的共享范围为域共享-全部，系统中的所有用户都可以使用域资源。
3. 单击 **_"确定"_** 按钮，完成操作。

### 调整调度标签

该功能用于为宿主机绑定调度标签，绑定调度标签的宿主机将按照调度策略调度创建虚拟机。当宿主机需要绑定同一个标签时，推荐使用批量为宿主机调整标签功能，若需要绑定不同标签，需要分别调整单个宿主机的调度标签。

**为单个宿主机调整标签**

1. 在宿主机页面，单击宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"调整调度标签"_** 菜单项，弹出调整调度标签对话框。
2. 选择调度标签，单击 **_"确定"_** 按钮。

**批量为宿主机调整标签**

1. 在宿主机列表中勾选一个或多个宿主机，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"调整调度标签"_** 菜单项，弹出调整调度标签对话框。
2. 选择调度标签，单击 **_"确定"_** 按钮。

### 调整超售上限

该功能用于设置宿主机CPU和内存的超售比以及系统预留内存，超售即宿主机提供超过自身拥有的CPU或内存资源，宿主机实际可分配资源为实际资源*超售比。一般情况下CPU超售比可以远大于1，内存超售比建议为1。

**单个宿主机调整超售上限**

1. 在宿主机页面，单击宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"调整超售比"_** 菜单项，弹出修改属性对话框。
2. 设置以下参数：
    - CPU超售比上限：设置宿主机CPU的超售比上限，宿主机可分配虚拟机CPU数量 = 宿主机的CPU数量 * 超售比。
    - 内存超售比上限：设置宿主机内存的超售比上限，宿主机可分配虚拟机内存 = （宿主机实际内存 - 系统预留内存 ）* 超售比。
    - 系统内存预留（GB）：设置宿主机的系统预留内存，最低为1GB。宿主机的预留内存将不会用于分配虚拟机使用。
3. 单击 **_"确定"_** 按钮。

**批量调整超售比**

1. 在宿主机列表中勾选一个或多个宿主机，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"调整超售比"_** 菜单项，弹出修改属性对话框。
2. 设置以下参数：
    - CPU超售比上限：设置宿主机CPU的超售比上限，宿主机可分配虚拟机CPU数量 = 宿主机的CPU数量 * 超售比。
    - 内存超售比上限：设置宿主机内存的超售比上限，宿主机可分配虚拟机内存 = （宿主机实际内存 - 系统预留内存 ）* 超售比。
    - 系统内存预留（GB）：设置宿主机的系统预留内存，最低为1GB。宿主机的预留内存将不会用于分配虚拟机使用。
3. 单击 **_"确定"_** 按钮。
### 宕机自动迁移

该功能用于设置{{<oem_name>}}平台的宿主机是否启用宕机自动迁移。宿主机启用宕机迁移后，宿主机上使用共享存储创建的虚拟机都可以在宿主机关机或故障时迁移到其他宿主机上。宿主机上使用宿主机本地存储的虚拟机不会迁移。

1. 在宿主机页面，单击宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"宕机自动迁移"_** 菜单项，弹出宕机自动迁移对话框。
2. 选择是否勾选自动迁移，单击 **_"确定"_** 按钮，完成操作。


### 进入维护模式

当宿主机临时下线时需要将宿主机进入维护模式，进入维护模式的宿主机上的虚拟机将自动迁移到其它宿主机上。仅{{<oem_name>}}平台宿主机支持。

{{% alert title="说明" %}}
宿主机进入维护模式的条件如下：

- 仅{{<oem_name>}}平台上的宿主机支持进入维护模式；
- 在{{<oem_name>}}平台上存在空闲的其他宿主机；
- 宿主机上虚拟机未挂载GPU设备或光盘；若宿主机上虚拟机已挂载GPU设备或光盘，需要保证虚拟机处于关机状态。
- 宿主机上虚拟机不存在备份机；
- 宿主机上虚拟机状态为关机、运行中或未知状态任意一种；

{{% /alert %}}

1. 单击宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"进入维护模式"_** 菜单项，弹出进入维护模式操作确认对话框。
2. 单击 **_"确定"_** 按钮，宿主机上的虚拟机将迁移到其它宿主机上，宿主机状态为”维护中“，启用状态为禁用。

### 退出维护模式

当宿主机恢复正常后，可将宿主机退出维护模式。仅{{<oem_name>}}平台宿主机支持。

{{% alert title="说明" %}}
宿主机进入维护失败时，可通过退出维护模式功能将宿主机的状态调整为运行。
{{% /alert %}}

1. 单击“维护模式”的宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"退出维护模式"_** 菜单项，弹出退出维护模式操作确认对话框。
2. 单击 **_"确定"_** 按钮，宿主机状态变为”运行中“，此时宿主机的启用状态为禁用，需要用户手动启用。

### 设置GPU卡预留资源

该功能用于在宿主机上为GPU卡预留CPU、内存、存储资源。预留的资源不能被分配出去。

{{% alert title="说明" %}}
- 仅带GPU卡的{{<oem_name>}}平台的宿主机支持该功能。
- 当宿主机上有多块GPU卡时，该功能即为每块GPU卡预留相同的资源。
- GPU卡预留的资源是宿主机CPU、内存、存储超售后的预留的资源。
{{% /alert %}}

1. 单击宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"设置GPU卡预留资源"_** 菜单项，弹出设置GPU卡预留资源。
2. 设置每个GPU预留资源，分别设置CPU、内存、硬盘大小，单击 **_"确定"_** 按钮。

### 删除

该功能用于删除宿主机。当宿主机上虚拟机数量为0，且处于禁用状态下才可以删除。

**单个删除**

1. 单击宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"删除"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。

**批量删除**

1. 在宿主机列表中勾选一个或多个宿主机，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"删除"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。

## Climc命令行操作

### 查询

通过 `host-list` 查询宿主机列表，`host-show` 查询宿主机详情。

```bash
# 查询 kvm 这种类型的宿主机
$ climc host-list --hypervisor kvm

# 查询被禁用的 kvm 宿主机
$ climc host-list --hypervisor kvm --disabled

# 查询启用的 kvm 宿主机
$ climc host-list --hypervisor kvm --enabled
```

### 启用

kvm 宿主机上线后，默认是禁用的状态，需要启用才能创建虚拟机。

```bash
# 找到禁用的宿主机
$ climc host-list --disabled

# 启用
$ climc host-enable <host_id>
```

### 禁用

如果完全不想让宿主机创建虚拟机，可以禁用它。

```bash
$ climc host-disable <host_id>
```
