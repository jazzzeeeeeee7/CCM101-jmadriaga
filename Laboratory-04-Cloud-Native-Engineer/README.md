# Mission 4: The Cloud-Native Engineer

## Mission Overview

This laboratory activity introduced me to containerization and Docker. I learned how containers are different from traditional virtual machines and how Docker can be used to run applications in a faster and more lightweight way.

## Objectives

- Understand the difference between virtual machines and containers.
- Check and verify Docker in the KillerCoda environment.
- Deploy an Nginx container using Docker.
- Practice basic Docker container lifecycle commands.
- Document the activities and results in GitHub.

## Docker Commands Executed

### Docker Verification

`docker --version`

This command checked the installed Docker version in the environment.

`docker info`

This command displayed information about the current Docker environment.

### Nginx Deployment

`docker pull nginx`

This command downloaded the official Nginx image from Docker Hub.

`docker run -d -p 8080:80 --name nginx-server nginx`

This command created and started the Nginx container in detached mode. It also connected port 8080 of the host to port 80 of the container.

`curl http://localhost:8080`

This command tested if the Nginx web server was running successfully.

### Container Lifecycle

`docker ps`

This command displayed the currently running Docker containers.

`docker stop nginx-server`

This command stopped the running Nginx container.

`docker ps -a`

This command showed all containers, including stopped containers.

`docker rm nginx-server`

This command removed the stopped Nginx container.

`docker ps -a`

This command was used again to verify that the Nginx container had been removed.

## Skills Learned

I learned how to use basic Docker commands for checking Docker, downloading images, running containers, and managing their lifecycle. I also learned how port mapping allows a service inside a container to be accessed through a port on the host.

## Challenges Encountered

One challenge I encountered was understanding how the Docker commands work together when creating and managing a container. Following the commands step by step helped me understand how to start, check, stop, and remove a Docker container.
