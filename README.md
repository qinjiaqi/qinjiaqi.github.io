## 自定义样式

博客主题fork自[Hux](http://huangxuan.me/huxblog-boilerplate/)，在UI 样式上做了较大的改动。

## 增加网易云音乐自选模块
![](http://www.soft568.com/UploadFile/2015-6/2015061512054749.jpg)

作为一个重度音乐患者，写文可以不配图，但是不能不配音乐啊。遂添加了网易云模块。这里要感谢网易云的分享机制，对开发者非常友好：

每首歌曲都支持生成外链播放器，且可以自定义显示尺寸。

网易云插件代码实例：
```
    <iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=86 src="//music.163.com/outchain/player?type=2&id=422428930&auto=1&height=66"></iframe>

```
对于不同的歌，唯一不同的是id号码。将上述`<ifram>`代码嵌入`post.html`文件中，记得放在合适的位置。另代码中的id改为：`id= {{ page.music-id }}`,同时在写好的markdown文档的头文件中添加：`music-id:*****`配置项。具体的id号就是选取的歌曲的外链中的id号。
