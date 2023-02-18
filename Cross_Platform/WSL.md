# Install WSL

安装步骤按照官方指引[使用 WSL 在 Windows 上安装 Linux](https://learn.microsoft.com/zh-cn/windows/wsl/install)即可。旧版Windows（所谓旧版我猜测是相对Win11的Win10，或Win10较旧的版本号）应参照[旧版 WSL 的手动安装步骤](https://learn.microsoft.com/zh-cn/windows/wsl/install-manual)。我的系统是Win10 19044版本，实际上基本是参考旧版安装指引来的。

这里仅列出安装过程中可能遇到的几个问题，以及解决方法。

- **启用Windows功能**   
    **控制面板->程序和功能->启用或关闭Windows功能**中有两项是必须启用的：
    - 适用于Linux的Windows子系统
    - 虚拟机平台

    勾选并点击确定后，可能会提示更新失败，导致后续无法[更新WSL2](https://learn.microsoft.com/zh-cn/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package)，这时可以先取消勾选点击确定，然后再次勾选点击确定。期间保险起见，要重启电脑。

- **启用Hyper-V**   
    同样在**控制面板->程序和功能->启用或关闭Windows功能**中要启用这一项，但奇怪的是我的功能列表中没有这一项（可能是以前不知道怎么卸载掉了），这时候需要手动安装Hyper-V，从网上摘抄了一段安装命令，保存为一个cmd文件后以管理员身份运行即可：
    ``` cmd
    pushd "%~dp0"
    dir /b %SystemRoot%\servicing\Packages\*Hyper-V*.mum >hyper-v.txt
    for /f %%i in ('findstr /i . hyper-v.txt 2^>nul') do dism /online /norestart /add-package:"%SystemRoot%\servicing\Packages\%%i"
    del hyper-v.txt
    Dism /online /enable-feature /featurename:Microsoft-Hyper-V-All /LimitAccess /ALL
    ```
    安装过程需要几分钟并重启电脑，之后功能列表中就会出现Hyper-V。

- **应用商店无法下载Linux**     
    错误代码：0x80072EFD，具体原因未知，这种情况只能手动下载安装包，官方提供的[Linux 发行版安装包](https://learn.microsoft.com/zh-cn/windows/wsl/install-manual#downloading-distributions)：
    - Ubuntu 22.04 LTS
    - Debian GNU/Linux
    - Kali Linux
    - Oracle Linux 8.5
    - ...
    
    下载后文件后缀可能是".zip"，手动改为".appx"然后运行即可。由于系统或机器原因，可能无法安装ARM版本，可以尝试安装x64版本的发行版。

- **启动Linux失败**     
    从开始菜单启动安装好的发行版，要等好久（正常的话立刻会弹出一个命令行窗口），最终返回错误代码：0x80072ee7，在PowerShell中输入`wsl -l -v`也查不到版本信息。  

    猜测是网络设置原因，这里提供一个不保证100%正确的（因为后面我把这个设置还原后也能成功启动Linux）解决方案：
    1. 打开**控制面板->网络和共享中心->更改适配器设置**
    2. 双击点开当前的**网络连接**（以太网或WLAN），点击**属性**
    3. 打开“**Internet协议版本4(TCP/IPv4)**”这一项
    4. 选择“**使用以下DNS服务器**”进行手动设置，
        - 在首选DNS服务器中输入：4.2.2.1
        - 在备用DNS服务器中输入：4.2.2.2

# Enjoy WSL✌️
一切就绪后，再次使用命令`wsl -l -v`查看已安装的Linux发行版：
``` cmd
PS C:\Users> wsl -l -v
  NAME      STATE           VERSION
* Ubuntu    Running         2
```
就可以正常使用了，从开始菜单点击发行版图标或安装一个Windows新开发的终端都可以启动系统。这里推荐使用[MobaXterm](https://mobaxterm.mobatek.net/)这个软件和Linux进行交互。
![MobaXterm](./img/MobaXterm.png)