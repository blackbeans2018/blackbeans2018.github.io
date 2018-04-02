---
layout:     post
title:      "Git 常用命令整理"
subtitle:   "\"git push -u origin master\""
date:       2018-03-28 21:47:00
author:     "BlackBeans"
header-img: "img/post-bg-2015.jpg"
catalog:    true
tags:
    - 常用工具
---

> "Time to start..."

###一、提交到主干的步骤：

1、`git status`  查看本地改动 

2、`git add **  `  添加本地改动到提交缓存区 

3、`git commit -m “**”`  提交本地缓存区内容

4、`git push origin master:refs/for/master`  发布到远程仓库评审
    （如不需要评审可直接 `git push origin master`） 

5、如果要合并多次提交
`git add * `后 `git commit —amend `然后`git push`

6、修改commit提交说明信息 
`git commit —amend`

**注意：一般一个分支原则上只有一个提交，除非合并到一个里面，否则最好本地拉一个分支出来修改，在该分支上提交**
7、本地拉个分支，并在本地分支提交
`git checkout -b iss53 origin/master
git push origin HEAD:refs/for/master`

**举个提交到分支的例子：**
![](https://raw.githubusercontent.com/blackbeans2018/blackbeans2018.github.io/master/img/resource/git-branch.jpg)

`git push origin local_jp:refs/for/idc_jp`

###二、废弃评审，重提:
`git reset —soft 提交代码之前的commit id 
git add 
git commit -m “” 
git push origin master:refs/for/master 
`
###三、拉代码时本地有修改
`git stash`      存到缓冲区 
`git stash pop`   拉回 

###四、关于分支
`git branch -a`        查看所有分支
`git branch`           查看本地分支
`git branch -r`        查看远程分支
`git branch -D br `    删除本地分支
`git checkout -b `     本地分支名x origin/远程分支名x，使用该方式会在本地新建分支x，并自动切换到该本地分支x。
`git fetch origin `    远程分支名x:本地分支名x，使用该方式会在本地新建分支x，但是不会自动切换到该本地分支x，需要手动checkout。
`git checkout master ` 切换回master分支




