# 个人的静态网页

很高兴来做个分享,其实我也想用英文来分享,因为我的普通话也不是很好,

不过我还没能力用英文分享,所以你们就将就听我讲普通话。


  我今天分享的内容是: 个人的静态网页 ( 通常人们用来写**个人博客** )

我们都知道每个网站都有自己的服务器,搞个服务器又是很麻烦的事。
所以，通常人们都不会以为可以免费拥有个人网站。

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
  然后进入 创建config.js
  ```javascript
    module.exports = {
    title: 'RaymondHone Share',  // 设置网站标题
    description : 'Personal'
  }
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