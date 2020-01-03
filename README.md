# 本地git上传远程仓库github
> 前提：创建并关联好ssh
## 第一种情景
*本地项目并不是从远程仓库clone的，两边都是新建的*
* git init
* git add hello.txt<br/>git commit -m "first commit"
* git remote set-url origin git@github.com:WxbMutong/wxb.git
* git pull origin master --allow-unrelated-histories(非常关键)
* git push origin master:master
## 第二种情景
*本地项目是从远程仓库clone的*
* git clone origin git@github.com:WxbMutong/wxb.git
* git add hello.txt<br/>git commit -m "first commit"
* git push origin master
