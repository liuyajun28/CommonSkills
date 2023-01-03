
wget获取安装包
wget http://nginx.org/download/nginx-1.22.0.tar.gz

将安装包拷贝到指定目录
cp nginx-1.22.0.tar.gz /usr/local

解压安装包
tar -zxvf nginx-1.22.0.tar.gz


配置
``` 
 cd /usr/local/nginx-1.22.0

 ./configure  --prefix=/usr/local/nginx --with-http_realip_module --with-http_sub_module --with-http_gzip_static_module --with-http_stub_status_module --with-pcre --with-http_ssl_module

``` 
``` 
make
``` 
``` 
make install
``` 


cd /usr/local/nginx/sbin
启动
./nginx

验证
浏览器访问http://localhost
