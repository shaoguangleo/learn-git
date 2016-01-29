#我们编程吧 之 git
**Version 0.2 $at$ 2016.01.29**

[TOC]

#Git 简介
Git是一个开源的软件，作者是大名鼎鼎的**Linus Torvalds**，写出**Linux**的那个哥们。

Git是一个专门用于做修改记录的程序，也被叫做**版本控制**软件。

## 安装Git
这个很简单。

 - Windows用户，参考[github@windows](windows.github.com)
 - Mac用户，参考[github@MacOSX](mac.github.com)
*Git不像别的软件，安装完成后不会在桌面上有个logo什么的，直接终端操作*

##设置Git
###查看git版本
在终端中输入`git --version`，比如我的输出为：

> git version 2.7.0

下面的设置主要是告诉git是哪位大神在用*git*。
###设定你的名字
`git config --global user.name "<yourname>"`
###设定你的邮箱
`git config --global user.email "<youremail@example.com>"`

#新建repo
##repo
repo可以理解为一个被跟踪的文件夹，其中的任何内容做的任何更改都会被记录在册。

##新建一个repo
比如我们的文件夹就叫做`hello-world`吧。
执行下列指令：

 - 新建文件夹`mkdir hello-world`
 - 进入文件夹`cd hello-world`
 - 初始化`git init`

看看初始化成功没有，输入指令**git status**，只要不显示*fatal: Not a git repository...*，那就OK了。

恭喜了，第一步成功了。

##新增提交更改
###新建一个文件
假设现在在刚才建立的文件`hello-world`中，如果没有就妥妥滴进来。

新建一个文件，比如`vim readme`，然后输入一些简单的内容，比如
> hello git.

###查看git状态
这里我们可以检查目前repo的各种状态，比如是否有过任何修改，命令为：

>git status

此时的输出应该是类似下面找个样子：

![git status](http://img.blog.csdn.net/20160128224205307)

###新增文件
此时我们就可以将readme文件添加到档案库里面去了。
>git add readme

**小技巧**如果当前文件较多，可以是用**git add .**来一股脑地把所有的文件都给新增了。

此时的输出应该是这个样子：

![git-add](http://img.blog.csdn.net/20160128225130107)

###提交文件
>git commit -m "Adding a readme file"

此时的输出应该是如下这个样子：

![git-commit](http://img.blog.csdn.net/20160128225204654)

###修改文件查看移动
在readme文件中新增一行，此时是用命令：
>git diff

可以看到如下输出结果：

![git-diff](http://img.blog.csdn.net/20160128225553471)




#更多信息
Hi，XDJM们，更多信息欢迎移步微信公众号letsProgramming.

![letsProgramming](http://img.blog.csdn.net/20160128231400788)
