git 命令大全（增删改）
A---本地仓库基本操作
1.git add ---添加到缓存区
2.git commit -m ""   ---提交到本地仓库
3.git status ---查看缓存区状态（查看和仓库同步情况）
4.git diff ---查看缓存区文件和仓库文件异同
5.git log ---查看提交日志记录
6.git log ---pretty=oneline ---以单行模式查看日志记录
7.git reset ---hard HEAD^ --返回到上一版本
8.git reset ---hard HEAD~100 --返回到之前100个版本
9.git reset ---hard 122ded --(注：122ded只是版本id的缩写)直接返回到指定版本
10.git reflog ---查看提交记录commit注释
11.git checkout -- fileName ---(注：fileName是文件名字包括后缀)当前文件撤回上一次状态，包括git add到缓存区，和commit提交到仓库的状态
12.git checkout masterName  ---(注：masterName是分支名称)切换到当前分支
13.cat fileName ---(注：fileName是文件名字包括后缀)查看文件内容
B---关联远程仓库
1.git remote add origin git@server-name:path/gitProName.git  --关联远程仓库
2.git push -u origin master --第一次推送master分支内容
3.git push origin master --每次本地提交完成（git commit -m ""之后），需要的话可以更新远程仓库
C---从远程仓库clone一个本地仓库
1.在远程新建仓库（见github略）
2.git clone git@server-name:path/gitProName.git

