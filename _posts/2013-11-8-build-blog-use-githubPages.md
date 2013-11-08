---
layout: post
title: 使用Github Pages搭建个人独立博客
categories: [git]
tags: [jekyll]
published: true
---

# {{ page.title }} #

{{page.summary}}


### 题记 ###
以前总是不喜欢写blog,倒不是自己不喜欢总结或者记录,只是把很多工作或者学习中的东西都记在了笔记上,先后折腾了Evornote,有道云笔记,麦库记事等,记下来的笔记也有上百篇了,不过都是基础的东西,心里更多的还是觉得写出来的blog还是要注意点质量的,其实说到底还是懒~.but!!!从今天开始我决定要开始正式持续的写blog了,这两天我还在思索着要不要买个自己的域名和空间,后来想了想还是先把blog写起,于是有了这个处女篇.

### GitHub Pages###
Git和GitHub我就不多做介绍了,至于GitHub Pages的使用,网上教程也很多,我相信只要是接触开发的都可以创建出来.今天我主要说的是创建好默认的Repository之后如何通过jekyll来配合你实现站点静态内容的操作



### 安装Jekyll ###
1.安装Jekyll需要提供Ruby的相关环境和依赖,我用的是centos5

	yum install  gcc c++ make flex autoconf zlib curl zlib-devel curl-devel bzip2 bzip2-devel ncurses-devel libjpeg-devel libpng-devel libtiff-devel freetype-devel pam-devel -y
编译ruby

	wget http://mirrors.ibiblio.org/ruby/1.9/ruby-1.9.2-p180.tar.gz
	tar -xvzf ruby-1.9.2-p180.tar.gz
	cd ruby-1.9.2-p180/
	./configure
	make && sudo make install
查看版本

	ruby -v
编译rubygems

	wget http://rubyforge.org/frs/download.php/76728/rubygems-1.8.25.zip
	unzip rubygems-1.8.25.zip
	cd rubygems-1.8.25
	ruby setup.rb
      注意这里有个坑,因为GFW的存在,你有可能连接不上http://rubyforge.org,这时候你可以看[这里](https://github.com/mojombo/jekyll/issues/1409)
2. 此时可以安装Jekyll了
	gem install jekyll

推荐:
1.http://beiyuu.com/github-pages/
2.http://hahaya.github.io/2013/06/26/build-blog-on-github.html  
  

