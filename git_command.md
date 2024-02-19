# GIT
## GIT流程
### 本地
GIT登陆(全局) -> GIT生成SSH密钥(全局) -> GIT本地仓库初始化 -> GIT新建本地分支 -> 添加文件至GIT暂存区 -> 添加文件至GIT存储区
### 远程
GIT远程仓库添加密钥 -> 连接GIT远程仓库 -> 新建GIT远程仓库 -> 上传GIT存储区文件
## GIT常用命令
GIT登陆

`git config --global user.name "你的Git账号"`

`git config --global user.email "你的Git邮箱"`

GIT生成SSH密钥

`ssh-keygen -t rsa -C "你的Git邮箱"`

GIT初始化

`git init`

查看GIT分支(必须在GIT本地仓库路径下查看)

```
git branch  #查看git本地仓库分支
git branch xxx  #新建本地分支
git checkout xxx    #切换本地分支
git branch -d xxx   #删除本地分支

git push origin xxx #新建远程分支
git push origin --delete xxx    #删除远程分支
```

添加文件至GIT暂存区

`git add xxx`

查看文件状态

`git status`

上传GIT暂存区文件至存储区

`git commit -m "xxx"`

查看GIT存储区文件

`git ls-files`

连接GIT远程仓库

`$ git remote add origin '你的远程仓库地址'`

上传GIT存储区文件至远程分支

`git push origin xxx`

拉取GIT远程分支

`git pull `

