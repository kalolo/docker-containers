# docker-containers

### Mysql
```
$docker pull mysql/mysql-server:5.6 || 5.7.26
$docker run --name mysql-5.6 -e MYSQL_ROOT_PASSWORD=docker -p 3306:3306 -d mysql:5.6
$docker run --name mysql-5.7 -e MYSQL_ALLOW_EMPTY_PASSWORD=yes -p 3306:3306 -d mysql:5.7
$docker start mysql-5.6
```

### Mysql 8
```
$docker pull mysql/mysql-server
$docker run --name mysql-5.8 -e MYSQL_ALLOW_EMPTY_PASSWORD=yes -p 3306:3306 -d mysql/mysql-server
$docker start mysql-5.8
```


### Mongo
```
$cd mongodb
$docker build --tag=mongo-v1 .
$docker run --name mongo-v1 -d -p 27017:27017 -d mongo-v1
$docker start mongo-v1
```

### PostgreSQL v11
```
$cd postgresql-11/
$docker-compose up -d
$docker logs -f postgre-v11
$docker exec -it postgre-v11 psql -U postgres
```

### Redis
```
$docker run --name redis-local -p 6379:6379 -d redis
$docker start redis-local
```

### Clickhouse
```
$cd clickhouse/
$docker-compose up -d
```

Execute client:
```
$cd clickhouse/
$docker-compose exec ch_server clickhouse-client
```

