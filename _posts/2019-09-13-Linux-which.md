---
title: 每日一Linux命令 - which
mathjax: true
key: 20190813whcih
tags:
- Linux
---
### 所有参数
1. -n 指定文件名长度，指定的长度必须大于或等于所有文件中最长的文件名。
2. -p 与-n参数相同，但此处的包括了文件的路径。
3. -w 指定输出时栏位的宽度。

### 常用参数
#### which xx
查找命令、文件路径
```
which ls
#ls='ls --color=tty'
#	/usr/bin/ls

which 20190813.log
```