# 彩虹表

彩虹表(Rainbow table)是用于加密散列函数逆运算的预先计算好的表，常用于破解加密过的密码散列。彩虹表常常用于破解长度固定且包含的字符范围固定的密码（如信用卡、数字等）。这是以空间换时间的典型实践，比暴力破解（Brute-force attack）用的时间少，空间更多；但与储存密码空间中的每一个密码及其对应的哈希值（Hash）实现的查找表相比，其花费的时间更多，空间更少。使用加盐的密钥派生函数可以使这种攻击难以实现。

&#x20;       一言以蔽之，彩虹表是一种破解用户密码的辅助工具。彩虹表以时空折中理论为基础，但并不是简单地“以空间换时间”，而是一种“双向交易”，在二者之间达到平衡。
