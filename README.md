#我们编程吧 之 git
[TOC]

#Git 简介
Git是一个开源的软件，作者是大名鼎鼎的**Linus Torvalds**，写出**Linux**的那个哥们。

Git是一个专门用于做修改记录的程序，也被叫做**版本控制**软件。

# 安装Git
这个很简单。

 - Windows用户，参考[github@windows](windows.github.com)
 - Mac用户，参考[github@MacOSX](mac.github.com)
*Git不像别的软件，安装完成后不会在桌面上有个logo什么的，直接终端操作*

# 设置Git
##查看git版本
在终端中输入`git --version`，比如我的输出为：

> git version 2.7.0

下面的设置主要是告诉git是哪位大神在用*git*。
##设定你的名字
`git config --global user.name "<yourname>"`
##设定你的邮箱
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

#新增提交更改
##新建一个文件
假设现在在刚才建立的文件`hello-world`中，如果没有就妥妥滴进来。

新建一个文件，比如`vim ready`，然后输入一些简单的内容，比如
> hello git.



##查看git状态
这里我们可以检查目前repo的各种状态，比如是否有过任何修改，命令为：
>git status
