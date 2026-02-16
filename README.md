# Docker

## Monolithic vs Microservices

## Traditional vs Vertualization vs Containerization

## What is Docker?

## Installation of Docker

## Docker Commands for Container Management

```shell
docker run [ContainerImage]     # to run a container
docker run -d [ContainerImage]  # to run a container in detached mode
docker ps               # to list running containers
docker ps -a             # to list all containers
docker create [ContainerImage]  # to create a container
docker start [ContainerID]     # to start a container
docker stop [ContainerID]      # to stop a container
docker rm [ContainerID]        # to remove a container]
docker rm -f [ContainerID]     # to force remove a container
docker run -p [HostPort]:[ContainerPort] [ContainerImage]  # to expose a port
docker exec -it [ContainerID] bash  # to attach / access to a container
docker run -P [ContainerImage]  # to expose all ports on random ports from 32768 to 61000
docker logs [ContainerID]   # to check container logs
docker stats [ContainerID]  # to check container resources
docker ps -a -q # to list all conatainer IDs
docker rm -f `docker ps -aq` # to remove all containers
docker cp/mv # Home Work
```

## Docker command for images

```shell
docker images           # to list docker images
docker image list       # to list docker images
docker image [subcommand]   # to work with images
docker image rm
```


## Docker commands for Networking

## Docker commands for Volume


## Dockerfile

Configuration file for docker images



## History

```shell
docker volume create student-db-vol
  219  docker volume list
  220  clear
  221  docker run -d -P -e MARIADB_ROOT_PASSWORD='redhat' --volume student-db-vol: 
  222  docker run -d -P -e MARIADB_ROOT_PASSWORD='redhat' --volume student-db-vol:/var/lib/mariadb mariadb 
  223  docker ps
  224  docker exec -it 961 bash
  225  clear
  226  docker run -d -P -e MARIADB_ROOT_PASSWORD='redhat' --volume student-db-vol:/var/lib/mysql mariadb 
  227  docker ps
  228  docker rm -f 961
  229  docker ps
  230  docker exec -it d52 bash
  231  docker ps 
  232  clear
  233  git clone https://github.com/shubhamkalsait/EasyCRUD.git
  234  cd EasyCRUD/
  235  ls
  236  git checkout cdec-b48
  237  clear
  238  ls
  239  cd backend/
  240  ls
  241  docker ps 
  242  docker inspect d525
  243  gp
  244  git pull origin cdec-b48
  245  clear
  246  docker build . -t shubhamkalsait1/easycrud-backend:v1
  247  docker images
  248  docker login
  249  docker push shubhamkalsait1/easycrud-backend:v1
  250  docker images
  251  cd ..
  252  cd frontend/
  253  ls
  254  ls -a
  255  cat .env 
  256  docker build . -t shubhamkalsait1/easycrud-frontend:v1
  257  docker push shubhamkalsait1/easycrud-frontend:v1
  258  docker images
  259  docker run -d -p 8080:8080 shubhamkalsait1/easycrud-backend:v1 
  260  docker ps
  261  docker logs 48e
  262  docker logs 48fe
  263  docker ps
  264  docker images
  265  docker run -d -p 80:80 shubhamkalsait1/easycrud-frontend:v1
  266  docker ps
  267  docker ps -a
  268  docker logs e3d
```
