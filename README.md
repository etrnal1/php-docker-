## Docker部署PHP环境
* PHP
* MySQL
* Nginx
* Redis

#### 安装docker
```linux
# curl -fsSL https://get.docker.com/ | sh
```
国内加速
```linux
# curl -sSL https://get.daocloud.io/docker | sh
```

#### clone
```linux
# git clone https://github.com/hteen/docker-lnmp.git
```

#### 安装docker-compose
```linux
# curl -L https://github.com/docker/compose/releases/download/1.8.0-rc1/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
# chmod +x /usr/local/bin/docker-compose
```

#### 启动
```linux
# cd docker-lnmp
# docker-compose up -d
Creating dockerlnmp_redis_1
Creating dockerlnmp_mysql_1
Creating dockerlnmp_php_1
Creating dockerlnmp_nginx_1
#
```
启动ok

#### 测试

> * phpinfo : http://localhost/index.php
> * mysql : http://localhost/mysql.php
> * redis : http://localhost/redis.php
