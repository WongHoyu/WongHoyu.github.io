---
title: 每日一Linux命令 - touch
mathjax: true
key: 20190718touch
tags:
- Linux
---
### 所有参数
1. -a 只更改访问时间
2. -c, --no-create	不创建任何文件
3. -d, --date=字符串	使用指定字符串表示时间而非当前时间
4. -f (忽略)
5. -h, --no-dereference	会影响符号链接本身，而非符号链接所指示的目的地(当系统支持更改符号链接的所有者时，此选项才有用)
6. -m 只更改修改时间
7. -r, --reference=文件	使用指定文件的时间属性而非当前时间
8. -t STAMP	使用[[CC]YY]MMDDhhmm[.ss] 格式的时间而非当前时间
9. --time=WORD 使用WORD 指定的时间：access、atime、use 都等于-a选项的效果，而modify、mtime 等于-m 选项的效果

**请注意，-d 和-t 选项可接受不同的时间/日期格式。**

### 常用参数
#### 1. 不带参数
创建文件
```
touch log2019.log
```
#### 2. -r
将xxx的时间更新成yyy的时间
```
touch xxx.log yyy,log
```
#### 3. -t
将xxx的时间更新成指定时间
```
touch -t 197001010000 xxx.log
```
