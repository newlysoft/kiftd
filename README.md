# kiftd——青阳网络文件系统 #
## 一款小型、便捷、开源的个人网盘系统。 ##

### 快速导航
* 外网访问太慢？可以转至国内托管地址进行下载： https://gitee.com/kohgylw/kiftd 
* 需要从github上浏览项目？可以访问github上的项目主页： https://github.com/KOHGYLW/kiftd

### 什么是kift?
* 您还在使用U盘分享软件么？
> 很不幸，U盘易丢，同时又无法兼容各种平台的文件系统，在需要大规模分享时--通过U盘拷贝简直就像是接力赛一样原始又低效。
* 您还在使用免费的公用网盘么？
> 时不时传来的网盘关停热潮令人担忧，而其由外人管理的特性则让您不敢轻易把隐私文件存放在上面。
* 您需要搭建起一款私人的网盘而苦于没有好的选择？
> 破解软件同样无法确保安全性，隐藏的病毒令人担忧。同时，多数已有的网盘服务器软件设计老旧、性能笨重、语言的障碍更是使用中不可忽视的问题。

### 现在，您可以选择kift了。

本应用的作者 _青阳龙野@kohgylw_ 相信：不仅仅是他本人，而是还有很多人都需要在局域网内自己搭建起一个属于个人或团体的网盘服务器系统，这样就可以让所有在同一局域网内的朋友、同事或学生去访问、上传或下载自己网盘上的文件--无论是不足1MB的doc文本，还是超过4GB的1080p视频。而且这种网盘的安装必须十分简单快速，界面要使用中文，且能够完全兼容Windows/Linux/Unix(包括Mac OS X)系统。

此外，这个网盘还应该像主流的免费网盘一样支持Mp4视频直接在线播放、pdf文档直接预览、图片直接查看功能。

--实际上，作者最初编写kift的目的就是为了能实现上述功能，毕竟作为老师的他需要时常在班级里分享文件给学生。在他成功弄丢了几次U盘之后，便萌生了利用闲暇时间设计一款这样的应用的想法。

_注：kift的解压即用版就叫做kiftd_

-------------------
### 只需抽出3分钟时间，您就可以在您自己的电脑上搭建出一个专业快捷的网盘服务器了。

* 马上下载本网盘服务器？请点击右上方绿色按钮“Clone or Download”，之后选择“Download ZIP”进行下载,也可以前往国内托管的下载地址： https://gitee.com/kohgylw/kiftd （码云）
* 在线阅读《说明文档》？请直接点击上方文件列表中的《说明文档》来在线预览，它是本应用的完全体说明说，您可以通过它来了解关于本应用的全部内容。
* 立刻获取开源代码？请访问本应用代码托管地址：https://github.com/KOHGYLW/KohgylwIFT （Github）
（_注：该资源是v1.0.1的源代码。v1.0.2版本的源代码将在近期整理好之后发布_）
* 使用中遇到问题？请将您的发现提交到 https://github.com/KOHGYLW/kiftd/issues (Github)
* 需要联系作者？请发件至 kohgylw@163.com 

-------------------
马上知道kift的优势：
* 安装快速，只需3分钟即可将网盘服务器安装完毕，解压就好，不能更快速了。
* 跨越平台，无论是Windows还是Linux又或是Mac，都能随时开启这个网盘服务器。
* 功能专业，不要被它看似“简单”的页面给蒙蔽了。kift在页面响应速度如丝般顺滑的基础上，具备着视频播放、PDF预览、图片查看等主流公共网盘所具有的功能。光是这一点，就已经很有吸引力了。
* 开源免费，爱护用户硬件设施从开源开始。此外它不会产生任何遗留，能够做到轻轻地走就如轻轻地来，卸载仅需删除文件夹，且不会和你卖萌。
* 快捷方便，kiftd的目标是让最小白的用户也能随时使用它，令传输文件毫无障碍。

-------------------

最新讯息：
### 新版本v1.0.2
新的kiftd v 1.0.2使用 Spring Boot 框架进行了重构，并全面升级了其功能，该版本建议所有用户升级体验。
新功能包括：
+ 真正的解压即用——点击鼠标、开启网盘。
+ 简单的操作界面——即使不看说明书，您一定也能把它启动起来。
+ 自定义的文件系统存储位置——现在，您可以自由选择将kiftd的文件系统存放在哪个位置了。
+ 加密认证——为了进一步确保用户的账户安全，kiftd加入了RSA加密技术以提高用户登录时的安全性，防止它们被网络窃听者盗用后危害用户安全（防止一锅端）。
+ 同级文件夹下多图片浏览——新版本采用了viewer.js开源框架实现图片的预览，可以对图片进行放大、旋转、全屏，播放、左右翻转、上下翻转……
+ 更加简单快捷的选中操作——您可以点击文件行来选中某一个文件，或是按住Shift键选中多个文件——然后进行批量删除或打包下载。
+ MP3音频在线播放——该功能基于APlayer播放器插件，kiftd现在不但能以列表形式播放同级目录内的所有音乐，还可以显示歌词、歌手和封面图片。
+ 更高效的ZIP压缩——全新的ZIP压缩组件ZT-ZIP替换了原本很初级的ZIP压缩过程，提高了压缩速度。经测试，对于一个370MB大小的MP4视频，kiftd对其压缩的耗时减少了4秒，速度提升达20%。
+ 增加了对IE8的支持（实验性）。这是一个很尴尬的功能：作者最终还是决定将其添加上，但不保证效果。他已经意识到让每个人都装一个chrome确实很难，且很多人连如何切换“极速模式”浏览都无从下手。
+ 一些性能上的和细节上的完善，使得kiftd更加可靠。

### 功能速览v1.0.2
>注：图中涉及资源均来源于网络，仅用于展示kiftd功能，版权归其作者所有。

+ 主界面
![主界面展示](http://m.qpic.cn/psb?/V102epzF1ea2hN/YQM*9LdIGsq3FUma*dyMnBkJGLUKvtfqsHqEMHpLkNU!/b/dDABAAAAAAAA&bo=pAg4BAAAAAADJ5I!&rf=viewer_4&t=5)
+ 视频播放
![Vadio](http://m.qpic.cn/psb?/V102epzF1ea2hN/602PtSWxOYx*RglE*LqYtKfcnaneZy98cYUKBg9sk5I!/b/dDEBAAAAAAAA&bo=oQg4BAAAAAADN4c!&rf=viewer_4&t=5)
+ 音乐播放
![Audio](http://m.qpic.cn/psb?/V102epzF1ea2hN/l98HGCikn.RzCU80faplH7hKvsgQEYsYRFzpAN5STHA!/b/dFoAAAAAAAAA&bo=pwg4BAAAAAADN4E!&rf=viewer_4&t=5)
+ 图片查看
![Picture](http://m.qpic.cn/psb?/V102epzF1ea2hN/avVkAHi6Foxk6WDaDpOYM2lpB3RLJhW.sspHbsgN8*c!/b/dGEBAAAAAAAA&bo=ogg4BAAAAAADhzQ!&rf=viewer_4&t=5)
+ PDF预览
![PDF](http://m.qpic.cn/psb?/V102epzF1ea2hN/VQ07hYkhZ96HbBILL14OU.EsOyIM2rImW6hBA4bQpg8!/b/dDMBAAAAAAAA&bo=ngg4BAAAAAADN7g!&rf=viewer_4&t=5)
+ 此外还有：打包下载、批量上传、用户权限管理等。

-------------------

2018-07-27 kohgylw@青阳龙野 作者保留著作权
