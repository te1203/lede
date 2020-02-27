# A guide for how to sync git to the upsteam
```shell
# 查看你的远程仓库的路径：
git remote -v

# 把coolsnowwolf/lede.git的仓库设置为你的upstream.
git remote add upstream https://github.com/coolsnowwolf/lede.git

git add -A 
# 或者 
git add filename
git commit -m "your note"
git push origin master
git status

# merge 的关键命令

# 抓取源仓库的更新
git fetch upstream

# 切换到 master 分支
git checkout master

# 合并远程的master分支
git merge upstream/master

git status
git push
```