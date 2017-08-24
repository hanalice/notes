## git 常用命令
```
# 查看远程origin信息
git remote show origin

# 查看本地所有分支
git branch -vv

# 关联远程分支到本地分支
git branch --set-upstream local_branch origin/remote_branch

# 删除remote 分支
git push origin --delete <branchName>

# 删除本地已经合并的分支
git branch -d <branchName>

# 删除本地尚未合并的分支
git branch -D <branchName>

# 删除tag
git push origin --delete tag <tagName>

# 此为默认方式，不带任何参数的git reset，即时这种方式，它回退到某个版本，只保留源码，回退commit和index信息
git reset –mixed <commit-ID>

# 回退到某个版本，只回退了commit的信息，不会恢复到index file一级。如果还要提交，直接commit即可
git reset –soft <commit-ID>

# 彻底回退到某个版本，本地的源码也会变为上一个版本的内容
git reset –hard <commit-ID>

```
