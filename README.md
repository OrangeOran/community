## 练习项目

### 1.git命令
$ git add .  
$ git commit -m""  
$ git push   

$ git status  
$ git commit --amend --no-edit


### 2.




### 其他
1、每次操作都需要输入用户名和密码感觉很繁琐，解决方法，在本地的工程文件夹的.git下打开config文件
添加：

[credential]
helper = store

或者在git bash 中执行（亲测）：git config --global credential.helper store

再输入一次用户名密码后就可以保存住了。

2、不行就用以下方法：

先用git拉一次东西，拉的时候会提醒你输入帐号的密码

输入正确的帐号和密码后，等东西拉完以后输入

git config --global credential.helper store

以后就不用输入帐号和密码了


