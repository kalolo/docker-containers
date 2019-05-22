# docker-containers

### Mysql
```
$docker pull mysql/mysql-server:5.6 || 5.7.26
$docker run --name mysql-5.6 -e MYSQL_ROOT_PASSWORD=docker -p 3306:3306 -d mysql:5.6 || 5.7.26
$docker start mysql-5.6
```

### Mongo
```
$cd mongodb
$docker build --tag=mongo-v1 .
$docker run --name mongo-v1 -d -p 27017:27017 -d mongo-v1
$docker start mongo-v1
```
