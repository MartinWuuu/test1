# Test repository of git


### 1，clone

就是相当于把整个项目复制到本地

`git clone git@github.com:username/repository_name.git `

### 2, add

当你修改过项目中的文件想要提交到分支中，需要先执行add命令，将文件放到缓存中，等待被提交。

` git add filename.md`

### 3, commit 

将缓存区等待提交的文件提交到分支中

`git commit -m 'commit message'`

### 4, add & commit

add和commit两个步骤可以合并在一起

`git commit -am 'commit message'`

### 5, push

将本地代码同步到远程仓库代码

`git push origin master`

### 6, pull

将远程代码更新到本地

`git pull origin master`