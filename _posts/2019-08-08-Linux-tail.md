---
title: 每日一Linux命令 - tail
mathjax: true
key: 20190808tail
tags:
- Linux
---
### 所有参数
1. -f 循环读取
2. -q 不显示处理信息
3. -v 显示详细的处理信息
4. -c<数目> 显示的字节数
5. -n<行数> 显示行数
6. -s, --sleep-interval=S 与-f合用,表示在每次反复的间隔休眠S秒 

### 常用参数
#### -f
循环读取(**查看日志时常用**)
```
tail -f 20190808.log
tailf 20190808.log
```

#### -n +X / -nX / -n -X
-n +X 从X行开始打印 / -nX  -n -X 作用相同 
```
tail -nX 20190808.log
tail -n +100 20190808.log
tail -n -5 20190808.log
```

#### -q
不显示文件名的文件头
```
tail -q 20190808.log
```

#### -s
配合 -f 使用，每次反复的间隔休眠S秒
```
tail -fs 20190808.log
```
