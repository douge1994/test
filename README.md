# test
git add .
git commit --amend --reset-author 时，会以 VIM 编辑器的形式打开如下内容的文件
# Your branch is ahead of 'origin/master' by 1 commit.
#   (use "git push" to publish your local commits)
#
# Changes to be committed:
#       new file:   helloworld.txt
#
esc + :wq

status 命令查看状态，并使用 push 命令向服务器提交。
git status
git push

删除远程仓库文件/文件夹 
git rm -r --cached fileName //只在缓存中删除对应的文件   -r删除文件夹 不加删除文件
//git rm filename(同时在缓存和物理存储中删除文件，慎用)
git commit -m ""
git push

恢复删除的文件/ 回退已经commit 的文件版本
git reset --hard commit'sId
查看commit的id 
git log   //近期版本
git reflog //历史版本<只要出现过的commit 都将出现>

回退版本 
git status 
git reset HEAD <file> 不加file 名，回退所有

在没有进行add操作的文件 让其回退到初始版本<丢弃工作区修改>
git checout -- 文件名 //--必须的

--------------------------------------
