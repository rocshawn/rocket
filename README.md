# rocket
学习搭建RPC框架


### 2.3 日志模块开发
首先传教项目：

日志模块：
```
1、日志级别
2、打印到文件，支持日期命名，以及日志的滚动
3、c格式化风格：打印日志比如整数拼接字符串的时候比较方便
4、线程安全
```

LogLevel:
```
Debug
Info
Error
```

LogEvent:
```
文件名、行号
MsgNo
进程号
Thread id
日期、时间精确到ms
自定义消息
```


日志格式：
```
[Level][%y-%m-%d %H:%M:%s.%ms]\t[pid:thread_id]\t[file_name:line][%msg]
```

Logger 日志器
1.提供打印日志的方法
2.设置日志输出的路径