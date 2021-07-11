# Chino Dev Box

前后端开发(部署)环境一键docker

内置了支持json的Rejson版本的Redis



内含：
- Mysql:
  - localhost:3306
  - username: root
  - password: chino
- PostgreSQL ：
  - localhost:5432
  - username: chino
  - password: chino
- MongoDB:
  - localhost:27017
  - username: root
  - password: chino
- Mongo Express:
  - localhost:8081
  - username: root
  - password: chino
- PgAdmin4:
  - localhost:4321
  - email: admin@chino.com
  - password: chino
- Redis(rejson):
  - localhost:6379
- Nginx:
  - localhost:80

## 配置

postgreSQL数据库初始化 sql 请放置在`./postgreSQL/base.sql`

postgreSQL数据初始化 sql 请放置在`./postgreSQL/data.sql`

mysql数据挂载点在`./mysql/data`

mysql配置文件位置在`./mysql/config`

静态文件请放置在`./web`

Nginx配置文件请放置在`./nginx`

## 启动

**前台**

```bash
docker-compose up
# or (newer version)
docker compose up
```

**后台**

``` bash
docker-compose up -d
```

**停止**

``` bash
docker-compose stop
```

**如需重置开发环境**

``` bash
# Stop all container
host> docker-compose stop
# Remove stopped container (important!)
host> docker-compose rm -f
# Start all container
host> docker-compose up
```



Happy hacking! :smiley:

