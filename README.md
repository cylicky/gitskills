# gitskills
git 上传代码，遇到的问题解决办法
OpenSSL SSL_connect: Connection was reset in connection to github.com:443
git config --global http.sslVerify false

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