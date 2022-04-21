# 开发手册
1. [下载安装配置 Protobuf](Protobuf.md)
2. [部署Mysql数据库脚本](../../distribution/conf/nacos-mysql.sql)
3. 配置文件
    1. 配置mysql数据库连接
    ```properties
    spring.datasource.platform=mysql
    db.num=1
    db.url.0=jdbc:mysql://127.0.0.1:43306/nacos?characterEncoding=utf8&connectTimeout=1000&socketTimeout=3000&autoReconnect=true&useUnicode=true&useSSL=false&serverTimezone=UTC
    db.user.0=root
    db.password.0=dmt.123
    ```
4. 配置启动参数
    ```
    -Dnacos.standalone=true
    ```
    [Configure Standalone Start Nacos](imgs/start.nacos.standalone.png)