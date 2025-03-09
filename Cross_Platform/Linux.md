# Awesome Linux

- [Commands Cheat Sheet](#commands-cheat-sheet)
- [Basic Tricks](#basic-tricks)


## Commands Cheat Sheet

最常用的50个命令，按使用频率从高到低排列：

| 序号 | 命令名称                                 | 说明                      | 参数说明                               | 示例                                   | 运行结果                |
| :--: | ---------------------------------------- | ------------------------- | -------------------------------------- | -------------------------------------- | ----------------------- |
|  1   | `ls` (list directory contents)           | 列出目录内容              | `-l`（长格式）、`-a`（显示隐藏文件）   | `ls -l /home`                          | 列出 `/home` 目录详情   |
|  2   | `cd` (change directory)                  | 切换工作目录              | 无                                     | `cd /var/log`                          | 切换到 `/var/log`       |
|  3   | `pwd` (print working directory)          | 显示当前目录路径          | 无                                     | `pwd`                                  | 输出当前目录路径        |
|  4   | `mkdir` (make directory)                 | 创建新目录                | `-p`（递归创建）                       | `mkdir -p project/docs`                | 创建嵌套目录            |
|  5   | `rm` (remove)                            | 删除文件/目录             | `-r`（递归）、`-f`（强制删除）         | `rm -rf tmp/`                          | 强制删除 `tmp` 目录     |
|  6   | `cp` (copy)                              | 复制文件/目录             | `-r`（递归复制）                       | `cp -r src/ backup/`                   | 复制 `src` 到 `backup`  |
|  7   | `mv` (move)                              | 移动/重命名文件或目录     | 无                                     | `mv old.txt new.txt`                   | 重命名文件              |
|  8   | `cat` (concatenate)                      | 查看/合并文件内容         | `-n`（显示行号）                       | `cat -n file.txt`                      | 显示带行号的文件内容    |
|  9   | `grep` (global regular expression print) | 文本搜索                  | `-i`（忽略大小写）、`-r`（递归）       | `grep -i "error" log.txt`              | 输出包含 "error" 的行   |
|  10  | `man` (manual)                           | 查看命令手册              | 无                                     | `man ls`                               | 显示 `ls` 的帮助文档    |
|  11  | `chmod` (change mode)                    | 修改文件权限              | `u+x`（用户添加执行权限）              | `chmod 755 script.sh`                  | 修改脚本权限为 755      |
|  12  | `sudo` (superuser do)                    | 以管理员权限执行命令      | 无                                     | `sudo apt update`                      | 更新软件包列表          |
|  13  | `apt` (Advanced Package Tool)            | Debian 包管理工具         | `install`、`remove`、`update`          | `sudo apt install nginx`               | 安装 Nginx              |
|  14  | `ps` (process status)                    | 查看进程状态              | `-aux`（显示所有进程）                 | `ps -aux | grep nginx`                 | 列出 Nginx 相关进程     |
|  15  | `top`                                    | 实时系统监控              | 无                                     | `top`                                  | 显示动态进程信息        |
|  16  | `kill`                                   | 终止进程                  | `-9`（强制终止）                       | `kill -9 1234`                         | 终止 PID 为 1234 的进程 |
|  17  | `touch`                                  | 创建空文件/更新文件时间戳 | 无                                     | `touch newfile.txt`                    | 创建空文件              |
|  18  | `find`                                   | 搜索文件/目录             | `-name`（按名称）、`-type`（类型）     | `find / -name "*.log"`                 | 查找所有 `.log` 文件    |
|  19  | `tar` (tape archive)                     | 打包/解压文件             | `-xvf`（解压）、`-cvf`（打包）         | `tar -xvf archive.tar`                 | 解压 `.tar` 文件        |
|  20  | `ssh` (Secure Shell)                     | 远程登录服务器            | `-p`（指定端口）                       | `ssh user@192.168.1.1`                 | 连接到远程主机          |
|  21  | `echo`                                   | 输出文本/变量             | `-e`（解析转义字符）                   | `echo "Hello World"`                   | 输出 "Hello World"      |
|  22  | `df` (disk free)                         | 显示磁盘空间使用情况      | `-h`（易读格式）                       | `df -h`                                | 以 GB/MB 显示磁盘使用   |
|  23  | `du` (disk usage)                        | 查看目录/文件大小         | `-sh`（汇总大小）                      | `du -sh /var`                          | 显示 `/var` 的总大小    |
|  24  | `head`                                   | 显示文件头部内容          | `-n 10`（显示前 10 行）                | `head -n 5 log.txt`                    | 输出文件前 5 行         |
|  25  | `tail`                                   | 显示文件尾部内容          | `-f`（实时追踪）                       | `tail -f /var/log/syslog`              | 实时查看日志更新        |
|  26  | `less`                                   | 分页查看文件内容          | `/keyword`（搜索）                     | `less large_file.txt`                  | 分页浏览文件            |
|  27  | `vim`                                    | 文本编辑器                | 无                                     | `vim file.txt`                         | 打开文件编辑            |
|  28  | `chown` (change owner)                   | 修改文件所有者            | `user:group`（用户和组）               | `chown root:root file`                 | 将文件所有者改为 root   |
|  29  | `scp` (secure copy)                      | 安全复制文件到远程主机    | `-r`（递归）、`-P`（端口）             | `scp file.txt user@host:/path`         | 复制文件到远程主机      |
|  30  | `ping`                                   | 测试网络连通性            | `-c 4`（发送 4 次请求）                | `ping google.com`                      | 显示网络延迟统计        |
|  31  | `wget`                                   | 下载文件                  | `-O`（指定输出文件名）                 | `wget https://example.com/file.zip`    | 下载文件到当前目录      |
|  32  | `curl`                                   | 传输 URL 数据             | `-o`（保存到文件）、`-I`（显示头信息） | `curl -o file.txt https://example.com` | 下载文件并保存          |
|  33  | `history`                                | 查看命令历史记录          | `-c`（清空历史）                       | `history`                              | 显示历史命令列表        |
|  34  | `alias`                                  | 设置命令别名              | 无                                     | `alias ll='ls -alF'`                   | 创建 `ll` 别名          |
|  35  | `uname` (Unix name)                      | 显示系统信息              | `-a`（全部信息）                       | `uname -a`                             | 输出内核和系统信息      |
|  36  | `which`                                  | 查找命令的绝对路径        | 无                                     | `which python`                         | 显示 Python 路径        |
|  37  | `whereis`                                | 查找命令及其相关文件      | 无                                     | `whereis python`                       | 显示 Python 相关路径    |
|  38  | `useradd`                                | 添加用户                  | `-m`（创建家目录）                     | `sudo useradd -m john`                 | 创建用户 `john`         |
|  39  | `passwd`                                 | 修改用户密码              | 无                                     | `passwd john`                          | 修改 `john` 的密码      |
|  40  | `su` (switch user)                       | 切换用户                  | `-`（切换环境变量）                    | `su - root`                            | 切换到 root 用户        |
|  41  | `ln` (link)                              | 创建文件链接              | `-s`（符号链接）                       | `ln -s /path/file link`                | 创建符号链接            |
|  42  | `crontab`                                | 定时任务管理              | `-e`（编辑任务）、`-l`（列出任务）     | `crontab -e`                           | 编辑定时任务            |
|  43  | `systemctl`                              | 管理系统服务              | `start`、`stop`、`status`              | `sudo systemctl start nginx`           | 启动 Nginx 服务         |
|  44  | `free`                                   | 显示内存使用情况          | `-h`（易读格式）                       | `free -h`                              | 以 GB/MB 显示内存       |
|  45  | `netstat` (network statistics)           | 显示网络状态              | `-tuln`（监听端口）                    | `netstat -tuln`                        | 列出监听端口            |
|  46  | `rsync`                                  | 高效文件同步              | `-avz`（归档/压缩/显示进度）           | `rsync -avz src/ dest/`                | 同步 `src` 到 `dest`    |
|  47  | `awk`                                    | 文本处理工具              | `-F`（指定分隔符）                     | `awk '{print $1}' file`                | 输出文件第一列          |
|  48  | `sed` (stream editor)                    | 流式文本编辑              | `s/old/new/g`（替换文本）              | `sed 's/foo/bar/g' file`               | 替换文件中的文本        |
|  49  | `ssh-keygen`                             | 生成 SSH 密钥对           | `-t rsa`（指定密钥类型）               | `ssh-keygen -t rsa`                    | 生成 RSA 密钥对         |
|  50  | `mount`                                  | 挂载文件系统              | `-t`（指定文件系统类型）               | `mount /dev/sdb1 /mnt`                 | 挂载磁盘到 `/mnt`       |

**说明**：  
1. **参数说明** 仅列出常用参数，更多参数可通过 `man` 命令查看。  
2. **运行结果** 因实际环境不同可能有所差异，部分命令未填充具体结果。  


## Basic Tricks