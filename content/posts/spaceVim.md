---
title: "SpaceVim安装配置记录：将vim升级为vim ide"
date: 2022-12-05T11:01:36+08:00
draft: false
---

SpaceVim 是一个社区驱动的模块化的 Vim IDE，以模块的方式组织管理插件以及相关配置， 为不同的语言开发量身定制了相关的开发模块，该模块提供代码自动补全， 语法检查、格式化、调试、REPL 等特性。用户仅需载入相关语言的模块即可得到一个开箱即用的 Vim IDE。

<!--more-->


## 安装

1. 安装一些前置依赖：

   * git

   * curl

   * 字体（不然vim界面显示会有些奇怪）：spaceVim依赖字体`font-hack-nerd-font`，但是个人更加喜欢`font-sauce-code-pro-nerd-font`，强烈推荐:

     ```shell
     brew install font-sauce-code-pro-nerd-font
     ```

     然后iterm中配置下使用这个字体：![](/images/spacevim-iterm.jpeg)

2. 安装spaceVim：`curl -sLf https://spacevim.org/cn/install.sh | bash`

3. 更新插件：`vim`，spaceVim会自动更新插件
4. 配置：`~/.SpaceVim.d/init.toml`
   1. spaceVim默认使用相对行号，大部分人应该都不习惯，修改配置：`relativenumber = false`

## 扩展

可以安装对应开发语言的扩展。比如[java](https://spacevim.org/cn/use-vim-as-a-java-ide/)、[go](https://spacevim.org/cn/use-vim-as-a-go-ide/)

## 使用文档

扩展升级支持的vim语法和操作特性：[传送门](https://spacevim.org/cn/documentation/)