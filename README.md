# serv00_script
Easy to use serv00 with script.

**一个用于 [简化Serv00的脚本集合] 。**

使用前请打开登录面板：Additional services -> Run you own applications

确认 Status 为 Enable

* serv00的运行环境为freebsd，它不能安装docker。
## 概述

`serv00_script` 是一个 [简化安装脚本]。它可以帮助用户 [快速地部署开发环境或者测试环境]。

重要的是，因为这些命令很好理解所以没有夹带私货的可能性。

## 安装

1.  将 `[serv00_script](https://github.com/legiorange/serv00_script.git)` 文件下载到您的本地机器，如果不想使用MrchrootBSD来拓展玩法就不用下载了。
    ```bash
    git clone https://github.com/legiorange/serv00_script.git
    ```

2.  （可选）执行 install_MrchrootBSD.sh 来获取伪ROOT权限(也就是你的子目录具有root权限)：

     ** 有安装 BASH 的可选项，你只需要修改脚本去掉符号 # 和(optional)一行**

    ```bash
    chmod +x serv00_script
    ```
    你可以新建一个 run.sh 来执行 ./mrchroot chroot /usr/local/bin/bash 指令来节省时间。
    
serv00 缺乏root权限，你必须利用MrchrootBSD来获得子目录的执行权限。

## 有用的指令

显示 开放端口 (在不记录端口的情况下是最常用的）
```bash
devil port
```

