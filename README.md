启动nginx：./objs/nginx<br>
ps aux|grep nginx<br>
gdb attach ${pid}
bt
killall -9 nginx
## mkcert创建自签名证书
mkcert -install
mkcert -CAROOT
mkcert www.aaa.com aiPlatform.dev localhost 127.0.0.1 ::1 43.139.87.74