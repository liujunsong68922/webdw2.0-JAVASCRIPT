# webdw2.0-JAVASCRIPT
JAVASCRIPT编写的WebDW2.0版本的客户端端，与webdw2.0-server配合使用。

由于WebDW2.0和WebDW1.0相比，架构上做了很大的调整，由原来的瘦服务器，胖客户端模式改变为胖服务器，瘦客户端模式，因此上客户端的JS代码得到了极大的简化。

从原理上讲，JAVASCRIPT编写的页面和JS代码可以直接通过拷贝发布的方式进行发布，但为了统一各项目的发布方式，统一将项目定义为JAVA Web项目，采用打包成为war包的方式进行发布。

1. 采用git clone方式获取到项目源代码
2. cd webdw-js
3. mvn clean package ，执行打包编译命令，将js,html等打包成一个war包，目前项目里不包含任何的JAVA代码
4. 将war包拷贝到tomcat/webapps/目录下，自动发布，默认tomcat监听80端口
5. 采用 http://localhost/webdw-js/index.html 访问JS编写的WebDW2.0客户端演示页面
