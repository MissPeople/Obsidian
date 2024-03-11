
# 配置

Git的设置文件为`.gitconfig`，它可以在用户主目录下（全局配置），也可以在项目目录下（项目配置）。

- `git config --list` : 查看当前git配置
- `git config -e [--global]` : 编辑git配置文件
- `git config [--global] user.name "name"` : 配置提交用户名
- `git config [--global] user.email "email"` : 配置提交邮箱地址
# 仓库管理

- `git init` : 初始化git仓库
- `git remote add [url]` : 添加远程仓库
- `git remote -v` : 查看所有远程仓库

# 分支管理

- `git branch` : 查看所有分支
- `git branch -r` : 查看所有远程分支
- `git branch -a` : 列出所有远程分支和本地分支
- `git branch [name]` : 创建一个新的分支
- `git checkout [name]` : 切换到一个分支
- `git merge [name]` : 合并一个分支到当前分支
- `git rebase [name]` : 将当前分支重新基于另一个分支
- `git branch -d [name]` : 删除一个分支
- `git branch [branch] [commit]` : 从指定commit新建一个分支
- `git branch --track [branch] [remote-branch]` : 新建一个分支，并与指定的远程分支建立追踪关系
- `git branch --set-upstream [branch] [remote-branch]` : 在现有分支与指定远程分支间建立联系
- `git cherry-pick [commit]` :选择一个commit，合并进当前分支
- `git push origin --delete [branch name]` : 删除远程分支

# 文件管理

- `git add [file]` : 将文件添加到暂存区
- `git reset HEAD [file]` : 撤销对文件的修改
- `git rm [file]` : 删除工作区文件，放入暂存区
- `git rm --cached [file]`: 停止追踪指定文件，但该文件会保留在工作区
- `git mv [file-original] [file-renamed]`: 改名文件，并放入工作区

# 查看历史


- `git log`: 查看提交日志。
- `git log [name]`: 查看某个分支的提交日志。
- `git log --oneline`: 只显示提交哈希和提交信息的第一行。
- `git diff`: 查看文件差异。
- `git show [commit-ish]`: 查看某个提交的详细信息。

# 代码提交

- `git commit --amend -m [message]` :使用一次新的commit，替代上一次提交，若代码未发生任何新变化，则用来改写上一次commit的提交信息
- `git commit --amend [file1] [file2]` : 重做上一次commit，并包括指定文件的新变化