## 初始操作：
  
  1.新建一个文件夹。在命令行中，使用命令，`git inin` 将此文件设置为一个`本地仓库`

  如果把文件夹删了 再git init的话 相当于另一个本地仓库了

## 本地公钥

  1.生成公钥：ssh-keygen -t rsa -C 邮箱号

  一路回车

  显示公钥：cat ~/.ssh/id_rsa.pub

  公钥是为了和远程仓库建立免费连接使用的，就不用每次提交代码什么的都要登录github账号