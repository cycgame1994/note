# git常用命令

---

# 1、设置用户签名

```bash
git config --global user.name 用户名
git config --global user.email 邮箱
```

# 2、初始化本地库

```bash
git init
```

# 3、查看本地库状态

```bash
git status
```

# 4、添加暂存区

```bash
git add filename
```

# 5、提交本地库

```bash
git commit -m "log" filename
```

# 6、查看历史版本

```bash
git reflog

git log
```

# 7、版本穿梭

```bash
git reset --hard version
```

# 8、分支操作

```bash
git branch -v # 查看分支

git branch 分支名    # 创建分支

git checkout 分支名  	# 切换分支

git merge 分支名 # 把指定分支切换到当前分支，
```

> 合并冲突时，编辑好冲突内容后，提交时候不带文件名
> 

# 9、远程仓库操作

```bash
git remote -v # 查看当前所有远程地址别名

git remote add 别名 远程地址 # 起别名

git push 别名 分支 # 推送本地分支的内容到远程仓库

git clone 远程地址 #将远程仓库的内容拉到本地

git pull 别名 远程分支名 # 将远程仓库对于分支最新内容拉下来后与当前本地分支直接合并

```

# 10、标签操作

```bash
git tag #列出所有标签

git tag [tagname] #创建一个标签

git push [shortname] [name] # 将标签推送到远程仓库

git checkout -b [branch] [name] # 检出标签
```