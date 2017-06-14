# jetty 在线实验环境

## 软件简介

软件基本信息，License，所属的类别，作用，特点等。
Jetty是一个纯Java的HTTP（Web）服务器和Java Servlet容器。虽然Web服务器通常与向人员提供文档相关联，但Jetty通常用于机器到机器通信，通常在较大的软件框架内。Jetty作为Eclipse基金会的一部分开发为一个免费开源项目。Web服务器用于Apache ActiveMQ，Alfresco，Apache Geronimo，Apache Maven，Apache Spark，Google App Engine，Eclipse，FUSE，Twitter的Streaming API和Zimbra等产品。Jetty也是开源项目的服务器，如Lift，Eucalyptus，Red5，Hadoop和I2P。Jetty支持最新的Java Servlet API（支持JSP）以及协议SPDY和WebSocket。

所属类别是服务器软件

特点：

1.易用性

2.可扩展性

3.易嵌入性

## 软件官网

https://en.wikipedia.org/wiki/Jetty_%28web_server%29

## Dockerfile 使用方法

### 如何使用
要在后台运行默认Jetty服务器，请使用以下命令：
```
$ docker run -d jetty
```
您可以通过访问http://container-ip:8080或https://container-ip:8443/浏览器进行测试。要将Jetty服务器暴露给外部请求，请使用端口映射，如下所示：
```
$ docker run -d -p 80:8080 -p 443:8443 jetty
```
这将将端口8080映射到容器内，作为主机端口80和容器端口8443作为主机端口443.然后，您可以访问http://host-ip或https://host-ip浏览器。

### 环境
图像中的默认Jetty环境为：
```
JETTY_HOME    =  /usr/local/jetty
JETTY_BASE    =  /var/lib/jetty
TMPDIR        =  /tmp/jetty
```
## 资源链接

- https://en.wikipedia.org/wiki/Jetty_%28web_server%29
