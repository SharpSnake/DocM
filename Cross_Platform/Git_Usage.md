# Git Usage

- **迁移本地仓库**
  
  本地已存在的仓库（例如之前从gitee克隆），完整地（包含所有提交记录）迁移到别的托管网站，以github为例：

    1. 在github上新建一个空仓库，README、gitignore和license都没必要初始化。得到此仓库的url：https://github.com/SharpSnake/xxx.git

    2. 设置本地仓库的远程地址，这里采用先删后加的覆盖策略：

        git remote rm origin
        
        git remote add origin https://github.com/SharpSnake/xxx.git
    
    3. 推送时遇到<font color=#FF0000 >"Support for password authentication was removed"</font>的错误，表示远程推送不再支持密码验证，改成token验证了，所以首先要在github上生成一个token：

        进入github的*Settings->Developer settings->Personal access tokens->Generate new token*，按页面提示生成即可。

        生成好的token（长度40左右，仅包含字母和数字）码一定要立刻记下来，这个页面仅显示一次。

    4. 推送本地仓库
    
        git push --mirror https://token@github.com/SharpSnake/xxx.git

        其中token替换成上一步生成好的码就可以了。
    
    5. 推送时遇到<font color=#FF0000 >"OpenSSL SSL_read: Connection was reset, errno 10054"</font>错误的解决办法：

        git config --global http.sslVerify "false"

- **推送失败的回滚**
    
    无法推送远程仓库，因为本地分支在远程分支的后面
    https://blog.csdn.net/imxiezy/article/details/124506162

- **to do**


