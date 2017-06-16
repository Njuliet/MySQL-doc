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
