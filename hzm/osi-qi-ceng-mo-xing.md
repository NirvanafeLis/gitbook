# OSI七层模型

维基百科定义：

> “OSI模型，即开放式通信系统互联参考模型（Open System Interconnection Reference Model），是国际标准化组织（ISO）提出的一个试图使各种计算机在世界范围内互连为网络的标准框架，简称OSI。”

1. <mark style="background-color:yellow;">**物理层：把网络连接在一起的物理手段 负责传送0与1的电信号**</mark>
2. <mark style="background-color:yellow;">**数据链路层：决定0与1的解读 分组方式**</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">相关协议:ARP协议</mark>
3. <mark style="background-color:yellow;">**网络层：引进一套新的地址——"网络地址" 使得我们能区分不同的计算机是否属于同一个子网络 建立主机到主机的通信**</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">相关协议：IP、ICMP协议</mark>
4. <mark style="background-color:yellow;">**传输层：有了MAC地址和IP地址 我们还需要一个参数 表示这个数据包到底供哪个程序来使用 这个参数就叫'端口' 实现端口到端口的通信**</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">相关协议：TCP、UDP协议</mark>
5. <mark style="background-color:yellow;">**会话层：负责建立和断开通信连接，以及数据的分割等传输相关的管理 （例：何时建立连接？何时断开连接？该保持多久的连接？）**</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">相关协议：SSL、TLS协议</mark>
6. <mark style="background-color:yellow;">**表示层：设备固有的数据格式与网络标准数据格式之间的转换 （接受不同的信息，例如文字流、图像、声音等）**</mark>
7. <mark style="background-color:yellow;">**应用层：针对特定应用的协议 网络服务与最终用户的一个接口**</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">相关协议：HTTP、FTP、DNS、DHCP等协议</mark>
