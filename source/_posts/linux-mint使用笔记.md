---
title: linux-mint使用笔记
date: 2016-04-21 15:21:34
tags: linux
---

**最近一直在用linux mint 重装了系统，从深度系统迁移到了mint, 记录一下， 一个系统从刚刚安装到我现在状态的过程**

1. 安装搜狗输入法
  + 去搜狗官网下载deb包
  + `sudo dpkg -i 搜狗输入法.deb` 或者直接双击就可以
  + 因为搜狗输入法依赖fctix,所以我又下载了个中州输入法
    `sudo apt-get install fcitx-rime && im-switch`
  + 安装完重启即可
2. 安装`oh-my-zsh`
  + 下载zsh： `sudo apt-get install zsh`
  + 下载安装oh-my-zsh： `sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
  + 改变默认bash: `chsh -s /bin/zsh`
