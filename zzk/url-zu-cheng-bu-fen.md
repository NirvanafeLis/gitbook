# url组成部分

一个完整的URL的组成由于：通信协议（scheme）、主机（host）、端口号（port）、路径（path）、查询（query）、信息片段（fragment）组成。 \
例如： \
https://www.baidu.com/?name=zs&\&age=15#middle \
拆解：\
scheme://host:port/path?query#fragment

```
scheme：通信协议，常用的协议http，ftp等。
host：主机，服务器（计算机）域名系统（DNS），主机名或IP地址。
port： 端口号，整数，可选，省略时是默认端口，如http的默认端口是80。
path：路径，由零或多个‘/’隔开的字符串，一般用来表示主机上的一个目录或者文件地址。
query：查询， 可选，用于给动态网页传递参数，可有多个参数，用“&”号隔开，每个参数的名和值用“=”号隔开。如：name=zs。
fragment：信息片段，字符串，锚点。
```
