# GIT使用

工作区 - 暂存区 - 本地仓库

1.在电脑上创建一个文件夹作为工作区
2.打开文件夹 -》右键git bash here进入当前目录
3.工作区持有项目实际文件

## readme文档
1.readme文件可以是txt文档，也可以是md文档
2.一般和项目放在一起，作为项目的说明文档

## 全局配置
1.配置用户名：git config --global user.name "你的git名称"
2.配置用户邮箱：git config --global user.email "你的git验证邮箱"
3.查看配置信息：git config --list

## 初始化
1.执行命令 git init 初始化版本库
2.当前目录路径后面有（master）表示初始化成功
3.在当前目录下会生成一个隐藏文件  .git  代表这是一个版本库
4.千万不能操作.git文件

## 把工作区内容提交到本地仓库
1.执行命令 git add 文件名  将工作区的内容提交到暂存区
2.命令git add .  将工作区所有修改提交到暂存区
3.执行命令git commit -m '提交注释'，从暂存区提交到本地仓库

## 辅助命令
1.命令 git status查看当前目录下的操作状态
2.git log 查看日志
3.git reflog 查看简版日志

## 回退版本(切记回退版本之前先提交当前修改的工作区，以免丢失已作的修改数据)
1.git reset --hard HEAD^(回退到上一个版本，一个^代表上一个版本)
2.git reset --hard 版本号 (回退到指定版本)

## 将本地仓库提交到远程仓库
1.在GitHub创建一个远程仓库
2.本地工作区先提交到本地仓库
3.本地仓库看链接远程仓库地址：git remote add origin '地址'
4.查看所关联的远程仓库：git remote -v
5.git push -u origin master 第一次执行
	git push 把本地仓库推送到远程仓库
	-u origin master 设置默认提交master分支到origin
6.git push -u -f origin master强制推送给远程仓库