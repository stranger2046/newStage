## 本地仓库操作

### 1、整理上一次提交

```
git commit --amend
```

git  commit --amend 作用主要在于：

1、让“本次Amend Commit的提交”覆盖掉最近一次提交的错误信息。并且gitk图形化界面上看不到被覆盖掉的错误信息记录，git log上也看不到被覆盖掉的错误信息记录。

2、如果想要查看“覆盖掉最近一次提交的错误信息”，可以使用git log加强版命令git reflog。如果想跳回“被覆盖掉的错误提交”，可以使用命令git reset --hard "commit_id"。

### 2、整理多次提交

```
git rebase -i h1 h2(左开右闭)
```

