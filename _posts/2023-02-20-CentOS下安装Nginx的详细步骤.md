[centOS7 安装nginx并启动 - 腾讯云开发者社区-腾讯云](https://cloud.tencent.com/developer/article/2080464)

安装步骤：

### 1、下载Nginx安装包

```bash
wget http://nginx.org/download/nginx-1.18.0.tar.gz
```

### 2、解压Nginx压缩包

```bash
tar zxvf nginx-1.18.0.tar.gz
```

### 3、进入Nginx目录下

```bash
cd /nginx-1.18.0
```

### 4、配置安装运行目录

```bash
./configure --prefix=/usr/local/nginx
```

### 5、出现如下错误需要安装依赖包

```bash
yum -y install pcre-devel

yum -y install openssl openssl-devel
```

### 6、进行重新配置

```bash
./configure --prefix=/usr/local/nginx
```

### 7、执行编译安装

```bash
make && make install
```

### 8、安装完毕，进入Nginx下的sbin目录并启动nginx

```bash
cd /usr/local/nginx/sbin

./nginx
```

eg:替换config文件

### 启动、停止的几个命令

#进入命令管理文件夹sbin

cd /usr/local/nginx/sbin



**#启动nginx**

./nginx

或

./nginx -c /usr/local/nginx/conf/nginx.conf



**#停止nginx**

./nginx -s stop



**#停止nginx(等待进程处理完毕进行关闭)**

./nginx -s quit



**#重启nginx**

./nginx -s reload
