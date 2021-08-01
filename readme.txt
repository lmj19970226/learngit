创建文件夹:mkdir filename
把当前文件夹初始化为Git管理的本地库：git init
添加到缓存区：git add readme.txt
上传到仓库：git commit -m "日志"
查看提交状态：git status
版本log：git log
log简介显示：git log -pretty=oneline
版本回退一个版本一个^：git reset --hard HEAD^
版本回退N个版本：git reset --hard HEAD~N
查看文件内容：cat readme.txt
查看整个版本历史：git reflog
回退到具体的版本号abcdefg的版本：git reset --hard abcdefg
查看文件夹下文件：dir
打开文件进行编辑：vi readme.txt
字母i或者a或者o进入可编辑状态；按ESC退出可编辑状态；
退出Vim编辑器ZZ大写或者wq或者wq!强制退出
查看文件被修改的内容：git diff filename
删除指定文件：git rm filename
删除文件夹：git rm -r --cached filename;然后commit；再push
提交到远程仓库：git push -u origin master
上传到远程仓库报错：Updates were rejected because the tip of your current branch is behin

hint: its remote counterpart. Integrate the remote changes
先尝试和远程仓库进行合并：git pull --rebase origin master再push
