进行安装git工具 sudo apt-get install git
先要创建一个目录, 这个目录就是用来存放仓库的  mkdir html  cd html
使用git init命令, 将当前目录创建成git仓库  git init
仓库创建成功了, 并提示这是一个空仓库 ls -al
创建一个文件README touch README
编辑这个文件, 写一点东西在里面 vim README
先用查看当前状态的命令, 查看一下现在目录下文件的状态 git status
把文件加到仓库中去, 只有加到仓库中了, 才可能看一下文件的变化 git add README
使用查看状态的命令, 看一下是目录下文件的状态 git status
进行提交 git commit
配置用户名 git config --global Njuliet
配置用户邮箱 git config --global cmj33441@outlook.com
配置编辑提交信息的编辑器 git config --global core.editor vim
查看一下提交的信息 git log
删除文件并查看 rm README ls ls -al
查看一下现在仓库是什么状态 git status
回复误删文件 git checkout README
回退到上次提交的版本 git reset --hard commitID
查看日志 git log
从仓库中删除文件 git rm filename
将删除提交到仓库 git commit
从版本库中忽略文件 touch .gitignore
版本之前对比 git diff commitID1 commitID2
git生成patch git format-patch -p1
git 打patch git am patch-name
创建分支 git branch branch-name
切换到新创建的分支上 git checkout -b branch-name
显示当前git仓库中有多少个分支 git branch -av
切换到分支  git checkout branch-name
一定要站在另一个分支上去删除它. 也就是说不能删除当前所在的分支 git branch -D branch-name
合并分支 git checkout master  git merge develop 如果出现冲突的时候可以使用mergetool, 解决冲突 git mergetool
使用tag命令来添加标签 是要创建标签的名称 git tag <tag-name>
若要删除标签，在tag命令指定 -d选项执行 git tag -d <tagname>
