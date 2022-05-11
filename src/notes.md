# 笔记



##### 本地分支上传远程分支操作步骤

1. 远程仓库新建分支dev
2. 本地仓库新建分支dev——git branch dev
3. 切换本地分支——git checkout dev
4. 修改提交到版本库后提交到远程分支——git push --set-upstream origin dev
5. 修改已被提交到远程分支dev



##### git pull 拉取代码报错

> error: some local refs could not be updated; try running
> 'git remote prune origin' to remove any old, conflicting branchesjie

解决方法：

1. git remote prune origin



##### 本地master分支提交到远程dev分支

```
git branch dev // 新建本地分支
git checkout dev // 切换本地分支
git add . // 提交修改到暂存区
git commit -m "commit content" // 提交修改到版本库
git checkout master // 切换本地主分支
git merge dev // 合并分支
git push origin dev:dev // 提交修改到远程dev分支
```