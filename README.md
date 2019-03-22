# 学习 git 时笔记
#### 参考 廖雪峰 大神的官方网站
## 里面有 git 的常用命令
## 如果你没有看过其他的 git 的话，其实会用 git 命令就已经可以了。
* git 原理
> 在本地上有一个 git 的本地仓库。这个需要用 git 指令与文件保持一致
>  删除后文件需要在 git 里  ---   git rm filename   ---
> 创建新的文件需要添加到 git 里   ---   git add filename ---
> 并且本地文件与本地库中间有一个 temp 仓库，需要 commit 才能将修改的变动提交到本地仓库里
### 常用方法
> 首先在你需要提交到库的文件夹的父文件中打开 git Bash here
> 第一次进入需要初始化 git 本地仓库  ---      git init
> 将你需要提交的文件添加到临时库中  ---   git add .   |   filename     ----   . 是添加所有文件   filename 是单个文件 ，可以添加多个单文件后再提交到本地仓库
> 将临时库中的文件添加到本地库中   ---  git commit -m "对这次提交描述"
* 将本地库中的文件推送至托管代码库中：github 或者 gitee 
首先需要关联远程的代码库 git remote add origin  ssh
然后就可以推送到远程库的 master：git push origin master