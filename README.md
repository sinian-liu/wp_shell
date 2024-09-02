# wp_shell
wordpress一键安装脚本
```
wget -N https://raw.githubusercontent.com/sinian-liu/wp_shell/main/main.sh && bash main.sh
```
安装完成后访问：
```
http://IP/wp-admin/install.php
```
卸载命令
1.停止 Docker 服务
```
sudo systemctl stop docker
```
2.删除 Docker 文件夹
```
sudo rm -rf /var/lib/docker
```
3.重新启动 Docker 服务
```
sudo systemctl start docker
```
4.这个命令将会搜索服务器上的所有目录，并列出所有包含 wp-config.php 文件的路径。
```
find / -name "wp-config.php" 2>/dev/null
```





## 引言
受够了无良的宝塔面板，无法忍受lnmp的龟速安装，快来试试wp_shell<br>
急速安装，全新的vps，五分钟内即可完成安装<br>
tips: aws 1h1g ubuntu20.04 实机安装时间为3分钟
## 使用教程
**目前只适用于自带apt软件包的系统, 如Ubuntu Debian**<br>
复制命令粘贴到vps里<br>
在执行过程中，出现了yes/no的交互，全都选y<br>
此脚本基于docker完成<br>
最后按照指引即可完成wordpress的安装<br>
注意初次访问要按ctrl+f5强制刷新一下网页
> 本程序适合没有建站基础的小白使用，大佬请回避
---
## license
MIT license
