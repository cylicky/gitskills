git config --global user.name ''  自己本地仓库的名称
git config  --global user.email '' 自己的邮箱地址

本地创建一个管理仓库
makdir name  创建文件
git init 把当前文件夹变成Git管理仓库
git add .   把文件添加到Git暂存区域
git commit -m '版本说明'  暂存区提交到本地库
返回消息
1 file changed：1个文件被改动（我们新添加的readme.txt文件）；
2 insertions：插入了两行内容

git reset --hard  '版本号'  切换版本号
git  log/reflog  查看版本号

git chenckout --file 撤回刚刚修改的文件
git status 查看文件状态

git reset HEAD . 撤回提交到暂存区的文件

git remote add origin 网上库路径 
git branch -M main 创建分支
git push -u origin main 上传到网上的分支

查看分支：git branch
创建分支：git branch <name>
切换分支：git checkout <name>或者git switch <name>
创建+切换分支：git checkout -b <name>或者git switch -c <name>
合并某分支到当前分支：git merge <name>
删除分支：git branch -d <name>