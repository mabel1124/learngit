初始化：git init
添加：git add <file>
          git commit -m <message>
工作区的状态：git status
查看修改内容：git diff
修改版本：git reset --hard commit_id
HEAD 指向当前版本
查看提交历史：git log
查看命令历史:  git reflog
查看工作区和版本库里最新版本的区别：git diff HEAD -- 
丢弃工作区的修改（未add）：git checkout -- file
丢弃暂存库的修改：git reset HEAD <file>
删除文件：git rm file
恢复最新版：git checkout -- file
关联远程库：git remote add origin git@server-name:path/repo-name.git
第一次推送master分支：git push -u origin master
提交远程库：$ git push origin master
查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>或者git switch <name>

创建+切换分支：git checkout -b <name>或者git switch -c <name>

合并某分支到当前分支：git merge <name>
合并分支（禁止ff模式）：git merge --no-ff -m"备注" name
删除分支：git branch -d <name>

当手头工作没有完成时，先把工作现场git stash一下，然后去修复bug，修复后，再git stash pop，回到工作现场；

在master分支上修复的bug，想要合并到当前dev分支，可以用git cherry-pick <commit>命令，把bug提交的修改“复制”到当前分支，避免重复劳动。

强制删除分支：git branch -D <name>