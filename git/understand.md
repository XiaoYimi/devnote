# Git 笔记

## 理解概念

- 远程仓库 Remote
- 本地仓库 Repository
- 暂存区 index
- 工作区 workspace



1. `远程仓库`可以理解为`存储在服务器上备份的代码`
2. `本地仓库`可以理解为项目包下 `.git所记录的提交记录`
3. `暂存区`可以理解为`目录或文件状态变动所标记的记录`
4. `工作区`可以理解`你所使用的开发编辑器`



## 理解命令

**符号理解**

```nginx
[]  表示可选指令
<>  表示必选指令
#   表示注释
```



- 初始化本地仓库

```nginx
git init [-y]

# -y 的作用: 简化操作
```



- 克隆项目

```nginx
git clone <http:xxx/username/xxx.git>
```



- 添加远程仓库地址

```nginx
git remote add orgin <http:xxx/username/xxx.git>
```



- 将当前分支改名为指定名称分支

```nginx
# ~project(main) 当前为 main 分支,改名为 master 分支
git branch -M master
```



- 查看项目目录或文件,以及文件内容状态变动情况

```nginx
git status
```



- 查看项目目录或文件,以及文件内容有哪些改动

```nginx
git diff

# 逐步使用 enter 键查看所修改的内容
# 按键 q 可退出查看,返回命令行操作面板
```



- 将所发生状态的目录或文件进行标记到暂存区

```nginx
git add .
# or
git add <指定文件路径>

# . 表示将所有状态变动的目录或文件都标记到暂存区
# 指定文件路径 => 是指在项目包里的文件路径

```



- 将暂存区所标记的内容提交到本地仓库

```nginx
git commit -m '备注提交信息(有利于冲突时的回滚恢复)'
```



- 拉取远程仓库((当前分支所在)的)源代码

```nginx
# ~project(master)
git pull

# 拉取 master 分支下的代码
```



- 将本地仓库的源代码提交到远程仓库

```nginx
git push [-u origin <branch>]

# -u origin <branch> 在首次提交到远程仓库时,建议指定远程仓库的提交分支,避免下次提交时重新寻址提交到指定分支
```



- 同步远程仓库分支到本地仓库

```nginx
git fetch
```







## 操作流程

![](C:\Users\Administrator\Desktop\devnote\git\git_command.png)