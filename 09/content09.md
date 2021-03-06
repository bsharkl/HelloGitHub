#### Python项目
1、[flask-limiter](https://github.com/alisaifee/flask-limiter)：flask limiter 是一个 flask 的扩展库，它可以根据访问者的 IP 限制其访问频率、次数等，示例代码如下：
```python
from flask import Flask
from flask_limiter import Limiter
from flask_limiter.util import get_remote_address

app = Flask(__name__)
limiter = Limiter(
    app,
    key_func=get_remote_address,
    global_limits=["2 per minute", "1 per second"],
)

@app.route("/slow")
@limiter.limit("1 per day")
def slow():
    return "24"

@app.route("/fast")
def fast():
    return "42"

@app.route("/ping")
@limiter.exempt
def ping():
    return 'PONG'

app.run()
```

2、[ngrok](https://github.com/inconshreveable/ngrok)：ngrok 是一个十分方便、好用的工具，它可以把本地某个端口的服务，通过一个安全隧道，映射到公网的一个地址。同时它提供了一个 web 页面，展示了每个请求、响应的所有信息，便于调试本地的程序。基本的使用方法如下：
```
ngrok 协议 本地服务监听的端口
ngrok http 8000

创建成功会返回公网地址，然后通过该地址就可以访问到本地的服务。
本地访问 http://localhost:4040，就可以查看关于每个请求、响应的相关数据
```

![](https://github.com/521xueweihan/HelloGitHub/blob/master/09/img/ngrok-show-min.png)

3、[glances](http://nicolargo.github.io/glances/)：glances 是一个可以让你**一目了然**你的系统情况（类top、htop)的工具，它界面友好，安装方便：`pip install glances`

![](https://github.com/521xueweihan/HelloGitHub/blob/master/09/img/glances-show-min.png)

#### Go项目
4、[lantern](https://github.com/getlantern/lantern)：lantern ——> 蓝灯vpn

#### PHP项目
5、[VulApps](https://github.com/Medicean/VulApps)：VulApps 是用于快速搭建各种漏洞环境，可用来学习、理解常见的漏洞，增强自己在开发过程的安全意识

#### Javascript项目
6、[vue-hackernews-2](https://github.com/vuejs/vue-hackernews-2.0)：这是一个Vue 2.0示例，克隆 [Hacker News]((https://news.ycombinator.com/)) 网站（我感觉比原站好看多了😅）

![](https://github.com/521xueweihan/HelloGitHub/blob/master/09/img/vue-hackernews-show-min.png)

7、[N-blog](https://github.com/nswbmw/N-blog)： N-blog 项目是面向新手的 Node.js 教程，该教程讲述了 Node.js 基本知识点，同时结合搭建一个多人博客的实战，从零基础到实际开发，由浅到深帮助新手入门 Node.js 这门语言

8、[pomelo](https://github.com/NetEase/pomelo)：pomelo 网易开源的一个Node.js游戏服务器框架，[Demo](http://pomelo.netease.com/demo.html)

#### C、C++项目
9、[json](https://github.com/nlohmann/json)：C++ 的 JSON 库

![](https://github.com/521xueweihan/HelloGitHub/blob/master/09/img/json-show.gif)

#### 机器学习
10、[machine-learning-for-software-engineers](https://github.com/ZuzooVn/machine-learning-for-software-engineers)：自上而下的学习路线: 软件工程师的机器学习，[中文版](https://github.com/ZuzooVn/machine-learning-for-software-engineers/blob/master/README-zh-CN.md)

#### Objective-C、Swift项目
11、[Kingfisher](https://github.com/onevcat/Kingfisher)：Kingfisher 是一个异步下载和缓存图片的库，你可以把它看做 SDWebImage 的纯 Swift 实现和替代。它可以帮助简单地实现像是用户头像或者 table view 里面的图片的下载和缓存这样的工作，以提高 app 速度和帮助开发者节省时间，[作者的中文博客](http://project.onevcat.com/)

#### Java项目
12、[MSEC](https://github.com/Tencent/MSEC)：MSEC 是腾讯开源的，毫秒服务引擎(Mass Service Engine in Cluster)
它是一个开源框架，适用于在廉价机器组成的集群上开发和运营分布式后台服务。毫秒服务引擎集RPC、名字发现服务、负载均衡、业务监控、灰度发布、容量管理、日志管理、key-value存储于一体，[官网介绍](http://haomiao.qq.com/index.html#documents)

## Android
13、[One Step](https://github.com/SmartisanTech/android)：One Step 是锤子开源的 Android 项目，一步（one step）是通过拖拽完成将信息发送至应用或联系人的动作，节省了在不同应用之间切换的诸多步骤，第一次打通了手持设备中应用间的边界，[One Step](http://www.smartisan.com/m1/#/os?section=onestep)

14、[android-open-project](https://github.com/Trinea/android-open-project)：Android 开源项目分类汇总

#### 其它

15、[freecodecamp](https://github.com/FreeCodeCampChina/freecodecamp.cn)：freecodecamp 是一个自由的开源编程社区，[freecodecamp中文社区](https://freecodecamp.cn)

16、[Web-Frontend-Introduction-And-Best-Practicesa](https://github.com/wxyyxc1992/Web-Frontend-Introduction-And-Engineering-Practices)：Web 开发入门与实践练习

17、[best-chinese-front-end-blogs](https://github.com/FrankFang/best-chinese-front-end-blogs)：该项目是收集优质的中文前端博客

18、[golang-open-source-projects](https://github.com/hackstoic/golang-open-source-projects)：中文版awesome-go

19、[Learn-Algorithms](https://github.com/nonstriater/Learn-Algorithms)：算法数据结构学习，C语言实现

20、[the-way-to-go_ZH_CN](https://github.com/Unknwon/the-way-to-go_ZH_CN)：《The Way to Go》中文译本，中文正式名《Go入门指南》

21、[FromXToGo](https://github.com/golang/go/wiki/FromXToGo)：如果你正从某个语言（PHP, Python, Ruby...）想要换到 Golang 却又害怕吗？（英文）

---
