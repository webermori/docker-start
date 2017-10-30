# docker-start
Learning Docker

## Basic commands

- docker ps: List containers
- docker run nginx
- docker stop nginx
- docker rm nginx
- docker run -d -p 8080:80 nginx
- docker run -d -p 8080:80 --name webserver nginx
- docker start webserver
- docker stop webserver
- docker exec webserver uname -a
- docker exec -it webserver bash

### Create DB
- docker run -d --name=dbserver -e "MYSQL_ROOT_PASSWORD=root" -e "MYSQL_DATABASE=docker-wordpress" mysql

### Access Database
- mysql -uroot -h dbserver -p
