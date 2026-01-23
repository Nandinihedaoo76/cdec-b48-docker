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




