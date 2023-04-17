# gitskills
Git is a version control system 


git config --global user.name 'ceshi_test'   自己告诉仓库你的名字
git config --global user.email '2906882615@qq.com'  Email地址

创建一个文件夹 mkdir test 
git init 把当前目录变成Git可以管理的仓库

git add .  把文件添加到Git 库把修改的代码放在暂存区

##Q：输入git add readme.txt，得到错误：fatal: not a git repository (or any of the parent directories)。

   A：Git命令必须在Git仓库目录内执行（git init除外），在仓库目录外执行是没有意义的。

##Q：输入git add readme.txt，得到错误fatal: pathspec 'readme.txt' did not match any files。

  A：添加某个文件时，该文件必须在当前目录下存在，用ls或者dir命令查看当前目录的文件，看看文件是否存在，或者是否写错了文件名。
git commit -m 'Git学习'  版本说明  暂存区所有文件提交到分支
1 file changed：1个文件被改动（我们新添加的readme.txt文件）；2 insertions：插入了两行内容

git reset --hard '版本号 commit'
git log  查看当前在那个版本，还有之前的
git reflog  查看所有版本号 

git status  查看修改的文件状态  红色代表修改过还没有放到暂存取，需要先 git add .  在从缓存区传上分支上 git commit -m '版本说明' 

cat 文件名  查看文件里面的内容  

git remote add origin https://github.com/cylicky/test_ceshi.git  链接网上库
$ git branch -M main      创建分支
$ git push -u origin main   上传到网上的分支上

git remote  add  origin 路劲
git push -u origin master  第一次提交
git push  origin master 后面提交

git status  查看状态

git add .  提交到缓存区，又修改了一次文件 
git checkout --file  撤回刚刚修改的文件

git reset HEAD 文件名  撤回提交上暂存区的文件

git status 插看文件状态

git remote  add  origin 路劲
git push -u origin master  第一次提交
git push  origin master 后面提交


git 上传代码，遇到的问题解决办法
OpenSSL SSL_connect: Connection was reset in connection to github.com:443
git config --global http.sslVerify false

 ## 使用git克隆github上的项目失败：unable to access github: OpenSSL SSL_read: Connection was reset, errno 10054
更新DNS缓存 
Windows  cmd终端  ipconfig /flushdns
MAC  sudo killall -HUP mDNSResponder    sudo dscacheutil -flushcache


##Q：输入git add readme.txt，得到错误：fatal: not a git repository (or any of the parent directories)。

   A：Git命令必须在Git仓库目录内执行（git init除外），在仓库目录外执行是没有意义的。

##Q：输入git add readme.txt，得到错误fatal: pathspec 'readme.txt' did not match any files。

  A：添加某个文件时，该文件必须在当前目录下存在，用ls或者dir命令查看当前目录的文件，看看文件是否存在，或者是否写错了文件名。




查看 
 1.查看clone 地址：git remote -v
 2.移除https的方式，换成ssh  git remote rm origin 
 3.添加SSH方式 git remote add origin '地址'

 
设置 秘钥
　A. 如果你也是初次使用码云，且没有设置过ssh key，请按照如下：
　1.键入：ssh-keygen -t rsa -C "你注册码云的邮箱" ，然后一路"Enter”
　2.打开：C:\Users\你的用户名/.ssh/id_rsa.pub
  3.复制：Notepad++打开上述文件，全部复制
  B. 添加公钥
  打开GitHub的Settings设置，接着打开SSH and GPG Keys，
  再点击New SSH Key按钮，title可随意填写，
  用记事本打开id_rsa.pub文件，将内容全部复制，
  然后粘贴到Key中，再点击add ssh key按钮
  
