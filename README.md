## 编译
```sh
./auto/configure --with-debug --with-http_ssl_module --prefix=/home/github/nginx --with-stream --with-ngx_stream_log_module 
```
启动nginx：./objs/nginx<br>
ps aux|grep nginx<br>
gdb attach ${pid}
bt
killall -9 nginx
## mkcert创建自签名SSL证书
mkcert -install
mkcert -CAROOT
mkcert www.aaa.com aiPlatform.dev localhost 127.0.0.1 ::1 43.139.87.74