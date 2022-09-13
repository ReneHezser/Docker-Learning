# Docker Quickstart

## Overview
This quickstart will show you basics about containers. We will not go deep into container development, but rather keep the focus on operating containers and understanding basic container concepts.

In the scenario you will be deploying a web application in a container environment. This shows how a typical application with a frontend and a backend (or database) can be deployed in a containerized environment.

![Architecture - Docker Containers](/assets/Architecture-Containers.jpg)

We will cover

- Create & build a container
- Run a container
- Troubleshoot containers
- Adding persistence to containers
- Docker networking
- Running a container without root permissions
- Build a multi architecture image
- Resource limits
- Container Orchestrators

The Quickstart has several challenges, that you are going to solve. They describe what, but not how to do it. If you see a little arrow like <details><summary>this</summary>

>```sample solution```
</details> then you can click on it and expand a sample solution for the task.

## Prerequisites
Before you start with the tasks, please make sure you've gone through them.
- [Comparing Container Runtimes: containerd vs. Docker](https://earthly.dev/blog/containerd-vs-docker/)
- [Introduction to Docker containers - MS Learn](https://docs.microsoft.com/en-us/learn/modules/intro-to-docker-containers/ )
- Docker Desktop installed / WSL / Azure VM

## Hosting an application in a docker container
In this step we create a new Dockerfile which customizes the basic Wordpress image, that is available on Docker Hub.

1. [Build the image](Steps/1.%20Build%20the%20image.md)
2. [Run the image locally](Steps/2.%20Run%20the%20image%20locally.md)
3. [Add a database](Steps/3.%20Add%20a%20database.md)
4. [Add Persistence](Steps/4.%20Add%20persistence.md)
5. [Networking](Steps/5.%20Networking.md)
6. [Run as non-root user](Steps/6.%20Run%20as%20non-root%20user.md)
7. [Add a second app](Steps/7.%20Add%20a%20second%20app.md)
8. [Change the image](Steps/8.%20Change%20the%20image.md)
9. [Multi-architecture images](Steps/9.%20Multi-architecture%20images.md)
10. [Resource limits](Steps/10.%20Resource%20limits.md)

Until now, we've started containers individually. The concept of a multi tier application (or microservices) has not been addressed.

## Container Orchestration

11. [Container Orchestration](Steps/11.%20Container%20orchestration.md)

## next Steps

- docker exec
- containerd commands
    - homework: what commands make sense for me?

## Sources

- https://www.serverlab.ca/tutorials/containers/docker/how-to-host-your-wordpress-site-with-docker/
- https://docs.docker.com/network/
- https://linuxhint.com/dockerfile_volumes/
- [Running a container with a non root user](https://betterprogramming.pub/running-a-container-with-a-non-root-user-e35830d1f42a)
- https://docs.docker.com/desktop/multi-arch/
- [Runtime options with Memory, CPUs and GPUs](https://docs.docker.com/config/containers/resource_constraints/)
- [Orchestration: What is Docker Swarm](https://programatically.com/orchestration-what-is-docker-swarm/)
- [Top 10 Logging Gotchas](https://sematext.com/blog/top-10-docker-logging-gotchas/)