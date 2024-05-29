# arping

**一、介绍**

ARP协议是“Address Resolution Protocol”（地址解析协议）的缩写。在同一以太网中，通过地址解析协议，源主机可以通过目的主机的IP地址获得目的主机的MAC地址。arping程序就是完成上述过程的程序。\
\
arping，用来向局域网内的其它主机发送ARP请求的指令，它可以用来测试局域网内的某个IP是否已被使用。&#x20;

**二、指令格式如下：**

```html
arping [-AbDfhqUV] [-c count] [-w deadline] [-s source] -I interface destination
```

**三、参数释意：**&#x20;

\-A：与-U参数类似，但是使用的是ARP REPLY包而非ARP REQUEST包。 \
\-b：发送以太网广播帧，arping在开始时使用广播地址，在收到回复后使用unicast单播地址。 \
\-c：发送指定的count个ARP REQUEST包后停止。如果指定了-w参数，则会等待相同数量的ARP REPLY包，直到超时为止。 \
\-D：重复地址探测模式，用来检测有没有IP地址冲突，如果没有IP冲突则返回0。 \
\-f：收到第一个响应包后退出。 \
\-h：显示帮助页。 \
\-I：用来发送ARP REQUEST包的网络设备的名称。 \
\-q：quite模式，不显示输出。 \
\-U：无理由的（强制的）ARP模式去更新别的主机上的ARP CACHE列表中的本机的信息，不需要响应。 \
\-V：显示arping的版本号。 \
\-w：指定一个超时时间，单位为秒，arping在到达指定时间后退出，无论期间发送或接收了多少包。在这种情况下，arping在发送完指定的count（-c）个包后并不会停止，而是等待到超时或发送的count个包都进行了回应后才会退出。 \
\-s：设置发送ARP包的IP资源地址，如果为空，则按如下方式处理： \
1、DAD模式（-D）设置为0.0.0.0； \
2、Unsolicited模式（-U）设置为目标地址； \
3、其它方式，从路由表计算。
