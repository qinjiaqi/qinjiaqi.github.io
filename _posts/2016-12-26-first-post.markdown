---
layout:     post
title:      "红红火火的首记"
subtitle:   "临近年终，seeu.cloud 上线啦啦啦啦。"
date:       2016-12-26 15:20
music-id:    22636871
author:     "QJQ"
header-img: "img/post-bg-2015.jpg"
tags:
    - 生活
---
## 前言

我这么无聊的人，难得的两个爱好：写字和guitar。

guitar是一直有认真在练习，有时候可以一个人一个曲子玩一整天。写东西却是看着哪天心情好，呼呼啦啦乱写一通，然后就不知道保存到哪里了。每每想找的时候要花好些时间。

最近思考了这个问题，确实不是什么好习惯，不认真对待的东西又怎么谈得上是喜欢呢。遂开发了`seeu.cloud`，想把写字这件事正儿八经的坚持下去，顺便显得“酷一些”。嘿嘿！

## 正文
开发`seeu.cloud`的过程不是很复杂，稍微有些编程经验的同学花上两天时间就能搞得定。
我选择了[GitHub Pages](https://pages.github.com/) + [Jekyll](http://jekyllrb.com/) 快速 Building Blog 的技术方案。毕竟用惯了**Markdown**和**Git**。方便、整洁、简单！

利用 GitHub Pages 的域名和免费无限空间，不用自己折腾主机。

默认的域名是`qinjiaqi.github.io`(把我的名字换成你的githubID)。如果想换成一个酷酷的域名，就需要去购买域名，再改改 DNS ，加个 CNAME 就OK。具体的操作网上教程很多。详情Google。

`seeu.cloud`这个域名我是在[GoDaddy](https://sso.godaddy.com/)购买的。每年50多块rmb。

博客主题fork自[Hux](http://huangxuan.me/huxblog-boilerplate/)，在UI 样式上做了较大的改动。

作为一个重度音乐患者，写文可以不配图，但是不能不配音乐啊。遂添加了网易云模块。这里要感谢网易云的分享机制，对开发者非常友好：

- 每首歌曲都支持生成外链播放器，且可以自定义显示尺寸。

- 网易云插件代码实例：

                <iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=86 src="//music.163.com/outchain/player?type=2&id=422428930&auto=1&height=66"></iframe>


对于不同的歌，唯一不同的是id号码。将上述`<ifram>`代码嵌入`post.html`文件中，记得放在合适的位置。另代码中的id改为：id= `{\{ page.music-id }\}`,同时在写好的markdown文档的头文件中添加：`music-id:*****`配置项。具体的id号就是选取的歌曲的外链中的id号。

我是在MarkEditor上码字的。这是一款很优秀的markdown编辑器。页面简洁大方，操作简单，还可以绑定七牛云账号，文档直接存到云端，不怕丢失。对了，目前是免费的，不过在编辑过程中会弹出注册码框。无碍。已入。

如果需要本地预览博客，需要下载`jekyll`，配置Raby环境。这些教程网上也是一大堆。就不赘述啦。



## 结语
`seeu.cloud`的意思很简单，**看你像看云**。

![](/img/see_cloud.gif)

小时候最喜欢的事情就是在秘密基地呆一下午。

躺在一大片青草地上，翘着二郎腿，叼一株狗尾巴草，哼着小调。

看云。

有风吹过来。

听奶奶在巷口喊自己名字。忙应一声。

翻身起来，高高兴兴回家吃饭。

······

我想如此这样温暖的回忆，便是我写字的缘由吧。
