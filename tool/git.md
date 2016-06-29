---
title: "Git"
date: 2016-06-10 15:59
collection: "版本控制管理"
---
#Git
@(GIT)[git,wiki]

[TOC]

##安装Git
```bash
git clone https://github.com/git/git
```

##创建远程代码库
相比于Github，BitBucket提供了不限制的私有代码库，这里也许更适合你。

1. 注册账号
2. 创建repository并记下代码库地址 https://guosichuan@bitbucket.org/guosichuan/mysimiki.git


##设置Git

设置用户名
```bash
git config --global user.name "guosichuan"
```

设置邮箱
```bash
git config --global user.email "guosichuan@gmail.com"
```

##创建本地代码库

初始化本地代码库
```bash
git init
```

加载所有项目文件
```bash
git add .
```

##提交文件

提交已加载的文件
```bash
git commit -m "initial commit"
```

询问git状态
```bash
git status
```

##创建分支

创建并同时切换到新建分支

```bash
git checkout -b new_feature
```

相当于

```bash
git branch new_feature
git checkout new_feature
```

查看项目下的分支

```bash
git branch
```

##合并分支
先加载并提交

```bash
git add .
git commit -m "adds my new feature"
```

移动到主干分支

```bash
git checkout master
```

合并到主干

```bash
git merge new_feature
```

##丢弃分支
加载并提交文件

```bash
git add .
git commit -m "feature to be discarded"
```

移动到主干分支

```bash
git checkout master
```

##删除一个分支
修改已经合并，从主干发送

```bash
git branch -d new_feature
```

修改未合并须强行删除

```bash
git branch -D new_feature
```

## 回滚

查看git 提交日志

```bash
git log
```

回滚到某一次提交（ID开头9个字符）

```bash
git checkout 085bb3bcb
```

也可以迁出一个旧版本的分支

```bash
git checkout -b my_previous_version 085bb3bcb
```

## 推送到远程代码库
第一次添加本地代码库到远程代码库

```bash
git remote add origin https://guosichuan@bitbucket.org/guosichuan/mysimiki.git
```
这里origin是别名，方便使用

之后推送主干分支到远程代码库

```bash
git push origin master
```

##取得远程代码库的一份拷贝
第一次拷贝
git clone https://guosichuan@bitbucket.org/guosichuan/mysimiki.git

更新版本

```bash
git pull origin master
```

##别名

```bash
git config --global alias.c 'commit -m'
git config --global alias.co 'checkout'
git config --global alias.cob 'checkout -b'
git config --global alias.br 'branch'
git config --global alias.m 'merge'
git config --global alias.a 'add .'
git config --global alias.s 'status'
git config --global alias.dbr 'branch -d'
```




