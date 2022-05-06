# 使用Docker部署Wordpress网站

- 安装docker
```
https://mirrors.tuna.tsinghua.edu.cn/help/docker-ce/
```

- 安装 docker-compose
```
https://docs.docker.com/compose/install/
```

- 克隆仓库
```
git clone https://github.com/zclongpop123/wordpress-docker.git
```

- 启动服务
```
docker-compose up -d
```

登录数据库管理
```bash
mysql -u root -p
```
创建数据库
```bash
CREATE DATABASE wordpress_db;
```
创建数据库用户
```bash
CREATE USER wordpress_db_user;
```
授予数据库用户权限
```bash
GRANT ALL ON wordpress_db.* TO  wordpress_db_user;
```
设置数据库用户密码
```bash
set password for wordpress_db_user=password("zcl.123");
```
