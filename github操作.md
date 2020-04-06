一、向本地仓库添加文件

0、创建文件夹并初始化

$ mkdir demo

$ cd demo

$ git init

1、创建文件

$ touch test.html

2、添加到暂存区

$ git add test.html

3、将文件从暂存区提交到仓库

$ git commit -m '添加test.html文件'

4、查看信息

$ git config --list

$ git status

二、将本地仓库代码推送到远程仓库

$ git remote add origin git@github.com:Ted163d/angular.git

$ git push -u origin master

(注：先从远程仓库克隆项目到本地仓库，对项目进行一系列操作后再push到远程仓库)

三、cnpm

安装：命令提示符执行
 `npm install cnpm -g --registry=https://registry.npm.taobao.org`

`cnpm -v` 来测试是否成功安装

四、清除克隆的git配置

rm -rf .git

git init

git status

git add .

git commit -m "提交"

git push git@github.com/Ted163d/angular.git

五、分支branch：

提示Your branch is up-to-date with 'origin/master' 该怎么办？

$ git branch newbranch

$ git branch

$ git checkout newbranch

$ git branch    //检查是否切换成功

$ git add .

$ git commit -m "提交信息"

$ git status

$ git checkout master

//将新分支改动合并到主分支

$ git merge newbranch

$ git push -u origin master

$ git branch -D newbranch    //删除分支





git学习完毕

