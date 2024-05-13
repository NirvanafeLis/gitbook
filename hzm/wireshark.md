# Wireshark



### 首先讲面板

wireshark有三个面板：

* packet list面板
* packet details面板
* packet bytes面板

这三个面板之间是相互关联的：

如果希望在packet details面板中查看一个单独的数据包的具体内容，必须在packet list面板中单机选中那个数据包 选中该数据包之后，才可以通过在packet deatils面板中选择数据宝的某个字段进行分析，从而在packet bytes面板中查看相应字段的字节信息

### packet list

packet list面板：以表格的形式显示了当前捕获文件中的所有数据报，从下面可以看出，一共有7列：

No（Number列）：包的编号 默认wireshark是按照数据包编号从低到高排序 该编号不会发生改变，即使使用了过滤也同样如此 Time列：包的时间戳。时间格式可以自己设置 Source列和Destination列：包的源地址和目的地址 Protocol列：包的协议类型 Length列：包的长度 Info列：包的附加信息

### packet details

packet details面板：分层的显示了一个数据包中的内容，并且可以通过展开或者收缩来显示这个数据包中所捕获的全部内容  默认数据详细信息都是合并的，如果要查看，可以单击每行前面的箭头：&#x20;

### packet bytes

packet bytes面板：

* 显示了一个数据包未经处理的原始样子，也就是它在链路上传播时的样子。
* 在该面板中的数据是以16进制和ASCII格式显示了帧的内容
* 当在packet details面板中选择任意一个字段后，在packet bytes面板中包含该字段的字节也高亮显示。
