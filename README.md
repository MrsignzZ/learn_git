# learn_git
git 学习项目

1. git 是以项目目录为单元的<br>
项目文件夹和文件，只有文件内容。<br>
文件版本，版本快照，<br>
文件具有了多个版本，git 就是一个版本控制协议。<br>
为了备灾，多人协作，中央远程代码仓库(github)<br><br>
commit id SHA-1(加密算法协议) 前六位代表它的ID<br>
HEAD 指针 master 分支 origin<br>
创建生成一条commit，id 为 xxx，指针指向本地的master，远程orgin指向主分支，远程HEAD
2. 。gitignore 哪些文件不上传<br>
node 类型
3. git clone 克隆<br>
git log<br>
cd .git 进入本地仓库
4. staged 暂存区 untracked file 未被追踪的文件(没有被写入暂存区)

<hr>

## GIT上传项目傻瓜式操作
  - 如果是上传文件到新的仓库
    1. github上先创建仓库
    2. git clone
    3. add commit push 三连

  - 如果是上传项目到新的仓库
    1. github上创建与项目同名的仓库(不要readme文件),如果创建了readme.md,要先拉取仓库的readme.md到本地 git pull --rebase origin master
    2. 项目根目录上git init
    3. git remote add origin + 仓库地址
    4. git add .
    5. git commit -m ""
    6. git push -u origin master