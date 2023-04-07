欢迎来到HTCPCD
==================

这是一个来自2013年的项目，来源于一个HTTP的一个梗：418 I‘m a teapot
由于这是一个来自十年前的的项目，且README是法语的。在十年后的今天我搜索到了这个项目，并且对他进行汉化。原 [项目地址](https://github.com/gelendir/htcpcpd)

HTCPCPD 是 HTCPCP 协议的实现
通过HTTP控制咖啡机。欲了解更多详情，请 [转到项目网页](http://gelendir.github.com/htcpcpd/)（当然，在今天这个网址已经404了）

HTCPCP 实施
==================================

Arduino的安装
-----------------------
要安装 Arduino 代码，只需通过 Arduino IDE 编译代码即可
并使用IDE将其传输到 Arduino。Arduino必须在一切中
与 HTCPCPD 服务通信时连接的时间。

服务器和客户端使用情况
------------------------------------

### 先决条件 ###

HTCPCPD服务端和客户端的唯一先决条件是已安装 Python 2.7。

### 安装 ###

对于服务器和客户端安装，您必须转到HTCPCPD的根目录，然后输入以下命令：

	python2 setup.py install

### 启动服务端 ###

要启动服务端，只需输入以下命令：
	
	htcpcpd -c htcpcpd.ini

其中“htcpcpd.ini”是配置文件。

配置文件所写的默认端口是8000。

配置文件中的“pidfile”表示HTCPCD服务的pid，方便结束HTCPCD的进程。

配置文件中的“logfile”用于设置HTCPCPD服务端日志位置。

### 启动客户端 ###

要使用客户端，只需输入以下命令：

	htcpcp-client localhost 8000

这两个参数都不强制性使用。第一个表示HTCPCPD服务端地址，第二个表示服务端端口。

### License ###

该项目使用 GPL V3许可
可在此处查看 : http://www.gnu.org/licenses/gpl-3.0.txt

