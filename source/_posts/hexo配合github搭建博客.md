---
title: hexo配合github搭建博客
date: 2016-04-16 16:48:05
tags: hexo　github
---
* 在本地搭建博客

  首先你电脑得装了node与npm，因为这个系统是基于nodejs的
  博客搭建的步骤只有五步
    ```bash

    npm install hexo-cli -g
    hexo init blog
    cd blog
    npm install
    hexo server

    ```

　至此你的博客已经搭建完成。并且能在localhost:4000端口可以访问

* 将博客推送到github
  + 配置github 修改blog里面的_config.yml,比如我的
  ```
    deploy:
    type: git
    repo: git@github.com:jackPanyj/jackPanyj.github.io.git
    branch: master
  ```
  其中我的repo填写的是ssh协议的，如果是https协议的话应该为`https://github.com/jackPanyj/jackPanyj.github.io`

  + 安装相关依赖:
  `npm install -S hexo-deployer-git`

  + 将博客推送到github：
  ` hexo d -g`

至此我的博客的访问地址应该是　`http://jackPanyj.github.io`
