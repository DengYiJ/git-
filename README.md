# git-
学习git用法
#  git操作

[TOC]



## 1.基本知识

分为四个区域

Workspace 工作区**

Index暂存区

Repository本地仓库

Remote ：gitee，github 等远程仓库**，推送到远程用PUSH

  ## 2.git创建版本库并提交文件

   git init  

   git add <FILE>

   git  commit -m"[^修改内容，更新的内容简述"]

  cat  <FILE>     [^看FILE 里面所有的信息]

  ## 3.git版本回退与追溯“未来版本”

  git log [^命令用于显示提交日志信息]

 git log -5 --pretty=oneline [^简化日志信息，显示最近期5行日志]

### git版本回退不同的表示语句

git reset --hard HEAD^  [^表明git回退到上一个版本，一个^表示一个版本、]

git reset --hard HEAD ~1 [^表明git回退到上一个版本，这次是不一样的表述方式，~能回退到很大数字的版本，如~100回退到上100个版本]

git reset --hard 版本标识符号            [^说明：打出前7个最为保险]

### git追溯”未来“版本（回到未来版本）

git reflog    [^  查看所有历史命令，能看之前引用位置]

git reset --hard 版本标识号     [^说明：跳到未来版本 ]      

 



## 4.文件删除

##    review：

1.git status 

2.git commit -m" 内容"

##    此节内容

git checkout -- <FILE>   [^ 将git区的文件，放回到工作区里，解决工作区（文件夹）误删的问题]

git rm  <FILE>   [^rm指remove，将文件从本地仓库中移除]

git ls-files [^查看本地仓库中所有文件]



## 5.远程操作

  ### 克隆远程项目到本地



