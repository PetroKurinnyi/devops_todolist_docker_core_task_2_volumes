## Creation of build of image for mysql

```
docker build . -t mysql-local:1.0.0 -f Dockerfile.mysql
```

## Starting container with mysql and volume

```
docker run -d --name my-sql-container -p 3306:3306 -v my-sql-volume-1:/var/lib/mysql mysql-local:1.0.0
```

## Build app image

```
docker build -t todoapp:2.0.0 .
```

## Start app container

```
docker run --name todo-app-container-2 -d -p 8080:8080 todoapp:2.0.0
```

## Link to app image on docker hub

https://hub.docker.com/r/petrokurinnyi/todoapp

## Link for opening app

http://localhost:8080/
