# GitHub 命令
```
git init                              #初始化仓库
git add                               #添加
git commit -m ''
git diff #比较本地与在线差别
git log
git log --pretty=oneline #输出日志文件
git reset --hard commit_id(id or HEAD^)
git checkout -- readme.txt
git reset HEAD readme.txt
```
---
git reset
HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令```git reset --hard commit_id(id or HEAD^)```。

穿梭前，用git log可以查看提交历史，以便确定要回退到哪个版本。
要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。
---
场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。

场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD file，就回到了场景1，第二步按场景1操作。

场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考版本回退一节，不过前提是没有推送到远程库。

---
git rm 删除后无法恢复

---

# 远程
```
git remote add origin git@github.com:trollchu/learngit.git
git push -u origin master

git clone git@github.com:trollchu/hello-world.git
```
