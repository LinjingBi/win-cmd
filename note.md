# 查杀进程      
- 查看所有网络进程占用的端口与PID
```
netstat -nao
```
- 对想看的端口做截取
```
netstat -ano|findstr "8080"
```
- 查看某PID的服务是什么进程
```
tasklist | findstr 2332
```
- 杀死进程
```
taskkill/pid 2332 -t -f
-f 用来强制执行
```
