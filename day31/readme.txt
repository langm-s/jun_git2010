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

4.查看配置信息：git config --list

## 初始化
1.执行命令 git init 初始化版本库
2.当前目录路径后面有（master）表示初始化成功
3.在当前目录下会生成一个隐藏文件  .git  代表这是一个版本库
4.千万不能操作.git文件

##把工作区内容提交到本地仓库
1.执行命令 git add 文件名  将工作区的内容提交到暂存区
2.命令git add .  将工作区所有修改提交到暂存区
3.执行命令git commit -m '提交注释'，从暂存区提交到本地仓库

##辅助命令
1.命令 git status查看当前目录下的操作状态
2.git log 查看日志
3.git reflog 查看简版日志