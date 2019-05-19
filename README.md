# 个人的静态网页
  我今天分享的内容是: 个人的静态网页 ( 通常人们用来写**个人博客** )

我们都知道每个网站都有自己的服务器,搞个服务器又是很麻烦的事。
所以，通常人们都不会以为可以免费拥有个人网站。

实现的方法其它很多,我这里是其中一种方法,

我总结了需要的资源：
> * github 帐号
> *  git 
> *  npm (安装Node.js即有)
> * vuepress 
### [vuepress中文网](http://caibaojian.com/vuepress/guide/getting-started.html)

举个例子:
  我做这个网页的时候,就先在github上创建一个分支叫 share
  然后在命令行进入share 执行
  ```
    vuepress build docs
  ```
  修改README.md 就是这个网页

  改完就在Git Bash 进入 share 执行
  ```
  vuepress build docs
  cd docs/.vuepress/dist
  ```
  然后提交到github 
  再部署:
  *如果发布到 https://**USERNAME**.github.io/**REPO***
  ```
  git push -f git@github.com:Raymond-Hong/share.git master:gh-pages
  ```


### [我的个人主页](https://raymond-hong.github.io)

### [本站源码地址](https://github.com/Raymond-Hong/share)