# git分支

## git分支切换

前提：先检查

```git
git status
```

已完成的保存

```git
git add ./<file name>
git commit -m
or
git stash
```

切换

```git
#切换分支
git checkout <branch name>
or
#新建并切换分支
git checkout -b <branch name>
```

当远程仓库没有分支时，提交新的分支

```git
自动补齐远程分支名字
git push <remote name> <remore branch name>
git push <remote name> <local branch name>:<remote branch name>
```

## git 推送方式从heeps转换为ssh

直接更改config文件的url

## 查看

```git
查看状态
git status
查看仓库信息
git remote	简单的分支列表
git remote -v	分支列表以及最后一次提交信息
git remote -vv	分支列表，最后一次提交信息，查看跟踪分支
查看本地分支
git branch -v
git branch -a
```

## 配置记住密码

```
永久记住密码
git config credential.helper store
默认记住15分钟
git config –global credential.helper cache
下面是自定义配置记住1小时
git config credential.helper ‘cache –timeout=3600’
```

## 贮藏工作

新的贮藏推送到栈上，运行 git stash 或 git stash push

查看贮藏的东西，可以使用 git stash list

将你刚刚贮藏的工作重新应用：git stash apply

## git从远程拉取本地不存在的分支

```git
//获取所有远程分支（不更新本地分支，另需merge）
git fetch

查看远程所有分支
git branch -a

查看所有本地分支，以及对应的远程分支，以及最后一次提交
git branch -vv

新建分支并切换到指定分支,并和指定的远程分支关联
git checkout -b <local branch name> origin/xxxxxxxx

将本地分支推送到远程
git push <远程主机名> <本地分支名>:<远程分支名>
```

## 