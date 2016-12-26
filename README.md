## 自定义样式

博客主题fork自[Hux](http://huangxuan.me/huxblog-boilerplate/)，在UI 样式上做了较大的改动。

## 增加网易云音乐自选模块
![](http://image.baidu.com/search/detail?ct=503316480&z=undefined&tn=baiduimagedetail&ipn=d&word=wangyiyun&step_word=&ie=utf-8&in=&cl=2&lm=-1&st=undefined&cs=1547414206,447587071&os=2090762607,1846553808&simid=3494136191,217195329&pn=23&rn=1&di=6120510001&ln=1986&fr=&fmq=1482750051489_R&fm=&ic=undefined&s=undefined&se=&sme=&tab=0&width=&height=&face=undefined&is=0,0&istype=0&ist=&jit=&bdtype=0&spn=0&pi=0&gsm=0&objurl=http%3A%2F%2Fbbs.htc.com%2Fcn%2Fdata%2Fattachment%2Fforum%2F201502%2F10%2F165634mtgzevxxwsupwaw1.jpg&rpstart=0&rpnum=0&adpicid=0)
作为一个重度音乐患者，写文可以不配图，但是不能不配音乐啊。遂添加了网易云模块。这里要感谢网易云的分享机制，对开发者非常友好：

每首歌曲都支持生成外链播放器，且可以自定义显示尺寸。

网易云插件代码实例：
```
    <iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=86 src="//music.163.com/outchain/player?type=2&id=422428930&auto=1&height=66"></iframe>

```
对于不同的歌，唯一不同的是id号码。将上述`<ifram>`代码嵌入`post.html`文件中，记得放在合适的位置。另代码中的id改为：`id= {{ page.music-id }}`,同时在写好的markdown文档的头文件中添加：`music-id:*****`配置项。具体的id号就是选取的歌曲的外链中的id号。
