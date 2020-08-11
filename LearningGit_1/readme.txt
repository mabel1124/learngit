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

删除分支：git branch -d <name>

