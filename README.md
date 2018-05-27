# 拍簧片Docker环境镜像
    PHP7.2.6 MySQL Nginx Redis
### 启动所有环境
    docker-composer.exe up -d
### 启动指定镜像
    docker-composer.exe up -d {package name}

### 目录说明
    project                     docker克隆目录
    ├─app                       网站项目目录
    |   |-default               默认网站目录
    |-mysql                     MySQL数据目录
    |-nginx                     Nginx配置目录
    |   |-vhost                 虚拟机配置目录
    |   |   |-test.conf         测试虚拟机配置
    │   │   └─ ...              更多虚拟机配置
    |   |-logs                  日志存放目录
    |   |   |-nginx             nginx日志目录
    │   │   |   |- access.log   nginx成功日志
    │   │   |   └─ error.log    nginx失败日志