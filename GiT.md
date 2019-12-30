## 配置
(1) 设置用户名与邮箱git config --global user.name "My Name"

git config --global user.email "my@email.com"

上面设置命令中带了“--global"参数，是全局配置，影响本机上所有的git项目。也可以对一些单独的项目进行设置，进入要设置的项目目录，进行设置：

cd dir

git config user.name "My Name"

git config user.email "my@email.com"查看配置：

cat .git/config

(2) 生成和添加 SSH Keys

由于git 也是客户端，服务端的模式，要想客户端可以和服务端通信，必须在客户端生成一个key(SSH Keys),然后添加到服务端去。


## 常用命令
克隆项目：git clone xxx.git 

创建分支：git branch daily/1.0.0

切换分支：git checkout daily/1.0.0

查看本地分支：git branch

查出远程分支：git branch -r

查看本地远程分支:git branch -a

创建并切换分支：git checkout -b daily/1.0.0

删除本地分支：git branch -d daily/1.0.0

强制删除本地分支：git branch -D daily/1.0.0

查看分支状态：git status

添加文件到git: git add file1 file2

添加所有文件: git add .

提交文件: git commit -m'注释'

拉主干：git pull origin master

合并主干：git merge master

更新分支：git pull -u origin daily/1.0.0

推送代码到远端：git push -u origin daily/1.0.0

打tag: git tag publish/1.0.0

发布到主干：git push -u origin publish/1.0.0
