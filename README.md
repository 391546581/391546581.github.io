https://zhuanlan.zhihu.com/p/492115006

hexo最简单的入门教程
枪打出头鸟
枪打出头鸟
​关注他
11 人赞同了该文章
​
目录
收起
1.hexo简介
2.项目展示
3.事前准备
4.快速入门
5.hexo项目结构
6.写作
7.安装主题
8.部署
其他
1.hexo简介
Hexo是一款基于Nodejs的，快速、简洁且高效的博客框架。具有丰富的插件和主题，具有超快的速度。支持Makedown语法，可以方便快捷的编写博客文档。同时支持node命令，可以一键部署到GitHub Pages, Heroku 或其他平台。

总之，是个写博客的利器。

2.项目展示
在介绍hexo如何使用前，先给你们看下我使用hexo搭建的个人博客—

锅锅的博客
​www.moyutime.cn/
3.事前准备
使用hexo前，首先要保证自己的电脑已经安装了Git 和 Node。且Node版本不低于10.13。

安装Git

- Windows：下载并安装git.

- Mac：使用 MacPorts或者下载安装程序

- Linux (Ubuntu, Debian)：`sudo apt-get install git-core`

- Linux (Fedora, Red Hat, CentOS)：`sudo yum install git-core`

安装Node

Node.js 为大多数平台提供了官方的 安装程序。

4.快速入门
1.安装hexo-cli

使用npm或者yarn安装hexo的脚手架工具，这里以npm为例

npm install -g hexo-cli
2.初始化项目

安装 hexo-cli 完成后，请执行下列命令，Hexo 将会在指定文件夹中新建所需要的文件。我们以新建一个hexo-demo项目为例进行说明。

hexo init hexo-demo
进入hexo-demo文件夹，安装依赖

cd hexo-demo
npm install
3.运行项目

安装完依赖以后，执行以下命令，启动hexo服务器，运行结果如图。

hexo server



在浏览器打开http://localhost:4000/ 就可以访问我们的博客了。

5.hexo项目结构
进入hexo-demo文件夹，我们可以看到hexo的目录结构，如下所示。

.
├── _config.yml
├── package.json
├── scaffolds
├── source
|   ├── _drafts
|   └── _posts
└── themes
接下来我们说下各个文件的作用。

_config.yml

_config.yml是整个博客网站的配置文件，里面包含了网站的配置、网址配置、目录配置、主题配置等等内容。

你可以根据自己的需要进行修改，我修改了网站配置、网址配置和主题配置，其他的使用默认。

默认的网站配置如下

网站配置

title: Hexo
subtitle: ''
description: ''
keywords:
author: John Doe
language: en
timezone: ''
修改成我们实际的配置

title: HexoDemo