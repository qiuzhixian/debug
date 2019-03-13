## [有哪些 JS 调试技巧？](https://www.zhihu.com/question/20260762)
- [移动端页面调试神器-browser-sync](http://www.cnblogs.com/kbqncf/p/4206244.html)
- [移动端前端开发调试](http://yujiangshui.com/multidevice-frontend-debug/)
- [如何在 PC 机上测试移动端的网页？](https://www.zhihu.com/question/20322475)
- [在手机上打印调试信息](https://github.com/binnng/debug.js)
- [微信调试、手机QQ调试、Qzone之x5内核inspect调试解决方案](https://blog.csdn.net/cengjingcanghai123/article/details/47001843)
- [打造最舒适的webview调试环境](https://div.io/topic/1449)
- [一探前端开发中的JS调试技巧](https://mp.weixin.qq.com/s?__biz=MzIxNzA4NzQ4OQ==&mid=403789355&idx=1&sn=0179c36bb89c473b460249b65d385916#rd&location=35)
- [针对手机网页的前端 console 调试面板](https://www.kancloud.cn/jsfront/month/160878)
- [移动WEB调试工具AlloyLever](http://www.alloyteam.com/2016/05/mobile-web-development-debugging-tools-alloylever-introduced/)
- [使用chrome开发工具远程在Android上远程调试](http://www.cnblogs.com/miss-radish/p/4990871.html)
- [微信内移动前端开发抓包调试工具fiddler使用教程](https://gaoboy.com/article/26.html)
- [活儿好又性感的在线 Mock 平台 - Easy Mock](https://zhuanlan.zhihu.com/p/26568521)
- [本地调试H5页面方案总结](https://www.jianshu.com/p/a43417b28280)

## 移动端webview常用的抓包方式：
https://blog.csdn.net/jingjingshizhu/article/details/80566191
https://www.cnblogs.com/zhongyanpingblog/p/4959190.html
### 一、Fiddle抓包
Fiddler是一个http协议调试代理工具，它能够记录并检查所有你的电脑和互联网之间的http通讯，设置断点，查看所有的“进出”Fiddler的数据（指cookie,html,js,css等文件）。 Fiddler 要比其他的网络调试器要更加简单，因为它不仅仅暴露http通讯还提供了一个用户友好的格式。
### [官网下载安装](http://www.telerik.com/fiddler)
### Fiddle配置
Fiddler的运行机制其实就是本机上监听 8888 端口的 HTTP 代理。
- 打开Fiddler,   Tools-> Fiddler Options 
- HTTPS，选中"Decrpt HTTPS traffic",    Fiddler就可以截获HTTPS请求
- Connections，选中"Allow remote computers to connect".  是允许别的机器把HTTP/HTTPS请求发送到Fiddler上来

### 手机配置
#### 安卓设置：
- 打开android设备的“设置”->“WLAN”，找到你要连接的网络，设置代理
- 在“代理”后面的输入框选择“手动”，在“代理服务器主机名”后面的输入框输入电脑的ip地址，在“代理服务器端口”后面的输入框输入8888，然后点击“保存”按钮。

#### IOS设置：
- 打开IPhone,  找到你的网络连接， 打开配置代理手动设置， 输入Fiddler所在机器的IP地址(比如:192.168.1.11) 以及Fiddler的端口号8888
- Fiddler证书安装(支持https)(打开IPhone 的Safari, 访问  http://192.168.1.11:8888， 点"FiddlerRoot certificate" 然后安装证书)

### 使用

### 二、[charles抓包](https://zhubangbang.com/charlesproxy)
支持修改线上代码，调试
- [Charles破解版免费下载和安装教程(含windows64位和Mac版本的破解文件)](https://zhubangbang.com/charles-crack-version-free-download-and-install-tutorial.html)
- [使用教程](https://zhubangbang.com/charles-the-phone-captures-the-package-setup.html)
- [手机安装CharlesSSL证书支持抓取HTTPS请求 chls.pro/ssl](https://zhubangbang.com/charles-https-packet-capture-method-and-principle.html)

### 三、[Thor抓包软件（ios）]()
- 安装
- 使用

### 四、[Packet Capture抓包软件（安卓）]()
- 安装
- 使用