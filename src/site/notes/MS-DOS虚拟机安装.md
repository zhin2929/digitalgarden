---
{"dg-publish":true,"dg-path":"笔记/MS-DOS虚拟机安装.md","permalink":"/笔记/MS-DOS虚拟机安装/","noteIcon":"","created":"","updated":""}
---


## 下载镜像
1. 可以选择去 [MSDN 我告诉你](https://msdn.itellyou.cn/) 下载，在搜索栏输入 ms-dos，点开详细信息，复制下载链接，用迅雷或其他支持该格式的下载软件下载。下载解压后需要用刻录软件将文件夹制作成软驱。此步骤略过，使用第二种方式直接下载软驱格式的 ms-dos 系统。
![MS-DOS 虚拟机安装1](/img/user/图片/MS-DOS虚拟机安装1.png)


1. [软驱格式 ms-dos](https://winworldpc.com/product/ms-dos/622) ，其实该步骤就是将第一种安装方式的过程做了。
![MS-DOS 虚拟机安装2](/img/user/图片/MS-DOS虚拟机安装2.png)

3. 有了 dos 系统的软驱后，安装 Virtual Box 软件，并创建一个虚拟机。
![MS-DOS 虚拟机安装3](/img/user/图片/MS-DOS虚拟机安装3.png)

![MS-DOS 虚拟机安装4](/img/user/图片/MS-DOS虚拟机安装4.png)

打开刚刚创建的 dos 虚拟机设置：
![MS-DOS 虚拟机安装5](/img/user/图片/MS-DOS虚拟机安装5.png)

添加 dos 系统的 img 镜像文件：
![MS-DOS 虚拟机安装6](/img/user/图片/MS-DOS虚拟机安装6.png)

分别添加 3 次全部选择进来：
![MS-DOS 虚拟机安装7](/img/user/图片/MS-DOS虚拟机安装7.png)
![MS-DOS 虚拟机安装8](/img/user/图片/MS-DOS虚拟机安装8.png)

![MS-DOS 虚拟机安装9](/img/user/图片/MS-DOS虚拟机安装9.png)

> [!warning] 注意 
> 然后启动，看到如下这个界面，此时直接按 Enter 进行安装会报错，从之前下载的文件名不难看出这个镜像是用来升级的，但是我们依然可以用它进行全新的安装，按两次 F3进入命令行模式。我们需要先对硬盘进行分区、格式化之后，才能进行安装。

![MS-DOS 虚拟机安装10](/img/user/图片/MS-DOS虚拟机安装10.png)

输入：`fdisk`，按 3 次回车键，重启后会回到安装界面。
![MS-DOS 虚拟机安装](/img/user/图片/MS-DOS虚拟机安装.png)

此时再按 2 次 `F3`，输入 `format C:` 在接下来的提示中输入 `y` 格式化 C 盘。至此，硬盘完成了分区和格式化。
![MS-DOS 虚拟机安装-2](/img/user/图片/MS-DOS虚拟机安装-2.png)

然后输入 `setup` 安装。看提示一路回车。来到这个界面后，提示说需要插入一张软驱。
![MS-DOS 虚拟机安装-3](/img/user/图片/MS-DOS虚拟机安装-3.png)

