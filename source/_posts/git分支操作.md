---

title: git分支操作

date: 2019-10-09 11:36:34

tags:

---

## 管理分支
<!--more-->
### 查看分支
1. 查看本地分支

使用 git branch命令，如下：

`$ git branch`
`* master`

*标识的是你当前所在的分支。
2. 查看远程分支

命令如下：

git branch -r

3. 查看所有分支

命令如下：

git branch -a

### 本地创建新的分支

命令如下：

git branch [branch name]

例如：

`git branch save`

### 切换到新的分支

命令如下：

git checkout [branch name]

例如：

`$ git checkout save`

### 创建+切换分支

创建分支的同时切换到该分支上，命令如下：

git checkout -b [branch name]

git checkout -b [branch name] 的效果相当于以下两步操作：

git branch [branch name]
git checkout [branch name]

### 将新分支推送到github

命令如下：

git push origin [branch name]

例如：

`git push origin save`

### 删除本地分支

命令如下：

git branch -d [branch name]

例如：

`git branch -d save`

### 删除github远程分支

命令如下：

git push origin :[branch name]

分支名前的冒号代表删除

例如：

`git push origin :save`