## Docker

* How do you have two different versions of a DB say MySQL 5.x and MySQL 8.x in a same machine?
* Installing and configuring a number of applications in your machine can be tedious

* Install **Docker Desktop**; Contains a Docker (Server or Engine or daemon); Docker Client (CLI, Visual)
* Using the client you connect to the server and create boxes (or containers)
* Each container is a Linux machine where your application is running

* docker pull <image>
* docker run <image>	

### Mysql

```
docker pull mysql:latest
docker run -p3306:3306 -e MYSQL_ROOT_PASSWORD=root mysql:latest
docker run -p3306:3306 -vYOUR_HOST_MACHINE_PATH:/var/lib/mysql  -e MYSQL_ROOT_PASSWORD=root mysql:latest

```