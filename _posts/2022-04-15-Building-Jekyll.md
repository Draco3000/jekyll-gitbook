---
title: Building Jekyll
author: Draco
date: 2022-04-15
category: code
layout: post
---
没想到 Jekyll + Github Pages 搞了三天才基本弄明白了，记录一些我常遇到的问题要点如下：

`gem install jekyll` 安装 Jekyll

`bundle add  webrick` 经常出现 LoadError 是因为没有安装webrick

`bundle install` 安装所有依赖包

`bundle exec jekyll serve` 排除有冲突的包强制启动 jekyll 本地 server---127.0.0.1:4000


对于使用新 Theme，最便捷的方法是直接 clone 对应的 Theme 的 repository 到本地，然后在这个文件夹里跑 Jekyll serve。

- 此外，图片资源应该在 repository 文件夹根目录里创建：
`docs/assets/images`

- 引用时使用：
`/repository-name/docs/assets/images`

