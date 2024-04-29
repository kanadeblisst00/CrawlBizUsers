## 文章链接

[aardio爬虫) 实战篇：采集自己的公众号粉丝列表](https://mp.weixin.qq.com/s/M9VYUyg_vYxXRa4KpFvlMg)

#### 功能介绍

虽然微信公众平台开放了API，但是很多接口订阅号都用不了，比如获取粉丝列表，不过我们可以在后台看到，那用爬虫也能实现。下面是大概的界面内容：

![](http://cdn.ikanade.cn/20240428204207.png)

界面只会显示当前页的内容，如果想看全部的数据，可以到当前文件夹下的`公众号粉丝.csv`里查看。采集的所有数据都会保存到里面（注意：如果还在采集你就打开的话，采集程序将无法保存到里面而失败）

#### 实现原理

使用webview2打开一个浏览器窗口让用户扫码登录公众号后台，然后获取cookies在使用kirequests请求库一直翻页请求。具体可以看上面那篇文章



