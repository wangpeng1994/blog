##一些名词
能解释命令行的就是shell，bash是升级版。

##文件的基本操作
- 创建
- 添加
- 修改
- 删除

##常见命令
####切换目录
|命令|含义|
|-|-|
|`pwd`|查看当前完整路径|
|`ls`|不包括隐藏文件|
|`ls -a`|查看当前目录下所有文件|
|`ls -al`|查看当前目录下所有文件的相详细信息|
|`cd`|cd代表切换路径|
|`cd .`|.代表当前文件夹|
|`cd ..`|..代表上一级文件夹|
|`cd /`|/代表根目录，最底层的路径|
|`cd ~`|~代表回到用户主目录|
|`cd Desktop/`|.代表进去桌面|
|`cd ~/Desktop`|代表回到用户主目录下面的桌面|
|`cd ~/Downloads`|代表回到用户主目录里的下载目录|

####创建删除文件
|命令|含义|
|-|-|
|`touch index.html`|创建html文件|
|`rm index.html`|删除html文件|
|`rm -r`|这样才能删除整个文件夹|
|`rm -rf`|彻底删除 不可恢复 没有询问|
|`mkdir projects`|创建文件夹 projects|

####重命名&移动文件
######（本质就是确认当前位置，找到目标文件移动到另一个目的地，同时可以重命名）
|命令|含义|
|-|-|
|`mv index.html INDEX.html`|重命名文件|
|`mv INDEX.html 123/`|移动文件到当前目录下的123文件夹内|
|`mv INDEX.html ..`|从123文件夹内移出到上一层|
|` mv ../INDEX.html index.html`|把上一层的INDEX.html文件移动到当前文件夹 并且重命名|
|` mv 123/index.html ~/Downloads/123.html`|找到123文件夹下的index.html，移动到家目录下的Downloads文件夹下，并且更名为123.html|

####编辑器vim
|命令|含义|
|-|-|
|`vim a.md`|初始进入编辑器命令模式，创建a.md|
|`i`或者`a`|进入编辑模式|
|‘esc’|进入命令模式|
|`:wq`|退出|
|`q!`|不保存强制退出|

####安装服务器
|命令|含义|
|-|-|
|`npm install http-server -g`|使用npm安装http-server，`-g`代表全局安装|
|`http-server`|开启服务器|

####文件权限
|命令|含义|
|-|-|
|`chmod 777 123.txt`|修改123.txt权限为当前用户&当前用户组＆其他人开启所有权限|
|`chown -R git:git zhangsan`|更改文件所属的用户和用户组|

##新手最大问题
* 大小写看错
* 空格写漏
* 把多个命令当成一个命令

##关于命令行的学习资料##
[每天一个Linux命令——竹子博客](http://www.cnblogs.com/peida/tag/linux%E5%91%BD%E4%BB%A4/default.html?page=4)
[npm 模块安装机制简介———阮一峰网络日志](http://www.ruanyifeng.com/blog/2016/01/npm-install.html)
* *  *
个人学习记录所用，如有错误，请评论区指出，谢谢~
