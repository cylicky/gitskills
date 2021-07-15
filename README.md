# gitskills
git 上传代码，遇到的问题解决办法
OpenSSL SSL_connect: Connection was reset in connection to github.com:443
git config --global http.sslVerify false

查看 
 1.查看clone 地址：git remote -v
 2.移除https的方式，换成ssh  git remote rm origin 
 3.添加SSH方式 git remote add origin '地址'
