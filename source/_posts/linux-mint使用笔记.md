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
3. 使用nvm安装node
  + 安装nvm： `curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.31.0/install.sh | bash`
  + 使nvm生效： `. ~/.nvm/nvm.sh`
  + 列出node的版本： `nvm ls-remote`
  + 安装node： `nvm install v5.10.1`
  + 设置为默认的版本： `nvm alias default v5.10.1`
