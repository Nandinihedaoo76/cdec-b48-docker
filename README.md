# Docker

## Monolithic vs Microservices

Monolithic vs Microservices Architecture
🔹 Monolithic Architecture

In a monolithic architecture, the entire application is built as one single unit.
All components such as UI, business logic, and database access are tightly coupled and deployed together.

Characteristics:

Single codebase

Single deployment unit

Components are tightly coupled

Scaling requires scaling the whole application

Advantages:

Simple to develop and deploy

Easy testing and debugging

Suitable for small applications

Disadvantages:

Difficult to scale individual features

Any small change requires full redeployment

Hard to maintain as application grows

Technology stack is fixed

🔹 Microservices Architecture

In microservices architecture, the application is divided into small, independent services.
Each service handles a specific business function and communicates via APIs.

Characteristics:

Multiple independent services

Separate codebase and deployment

Loosely coupled components

Each service can scale independently

Advantages:

Better scalability

Faster development and deployment

Easier maintenance

Supports multiple technologies

Disadvantages:

Complex architecture

Requires service communication management

Difficult debugging and monitoring

Needs DevOps and automation tools

🔹 Key Differences
Feature	Monolithic	Microservices
Architecture	Single unit	Multiple small services
Deployment	One-time deployment	Independent deployments
Scalability	Scale whole app	Scale individual services
Maintenance	Difficult for large apps	Easier for large apps
Technology	Single stack	Multiple stacks
Failure Impact	Entire app affected	Only affected service
🔹 When to Use

Monolithic: Small projects, startups, simple applications

Microservices: Large applications, cloud-native, high scalability needs
## Traditional vs Vertualization vs Containerization

## What is Docker?

## Installation of Docker

## Docker Commands

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
```
