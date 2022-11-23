## 本地公钥

  1.生成公钥：ssh-keygen -t rsa -C 邮箱号

  一路回车

  显示公钥：cat ~/.ssh/id_rsa.pub

  公钥是为了和远程仓库建立免费连接使用的，就不用每次提交代码什么的都要登录github账号

  然后，就可以在 `github` 或 `gitLab` 账号设置里面 `Settings` 中的 `SSH and GPG keys` 选项中

  new SSH key，将本地的公钥添加到里面即可

## 初始操作：
  
  1.新建一个文件夹。在命令行中，使用命令，`git init` 将此文件设置为一个`本地仓库`

  如果把文件夹删了 再git init的话 相当于另一个本地仓库了

  2.一般将本地仓库与远程仓库 建立链接的话操作如下：

```markdown
  1.首先在你们github账号下，创建一个远程仓库，建议先不要加入 README.md 文件。就是直接配置一个仓库名，和是否公共，还是私有 一个空的仓库就可以。

  2.使用命令：`git remote add origin git@github.com:Cluckyhy/Git_Basics.git`

  3.然后，就可以在本地仓库，写你的代码，或者其他操作（创建 README.md文件 .gitignore文件）

  4.使用 git add . 将新加的代码或文件。添加到缓存区

  5.使用 git commit -m '注释文字' 提交到本地仓库

  6.`第一次`将本地仓库推送到远程仓库，使用 `git push -u origin master`，
  
  只要做了第一步操作，将本地仓库和远程仓库建立好链接后，除了第一次推送，后面都只需要使用使用 `git push` 就可以了

```