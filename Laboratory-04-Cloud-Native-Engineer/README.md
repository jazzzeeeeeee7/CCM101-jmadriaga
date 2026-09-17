# Mission 4: The Cloud-Native Engineer

## Mission Overview

This laboratory activity introduced me to containers and Docker. I learned how containers differ from traditional virtual machines and how Docker can be used to deploy applications quickly.

## Objectives

- Understand the difference between virtual machines and containers.
- Verify Docker in the KillerCoda environment.
- Deploy an Nginx container.
- Use Docker commands to manage a container.
- Document the activities in GitHub.

## Docker Commands Executed

### Check Docker
-bash
docker --version
docker info

## Deploy Nginx
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080

## Container Lifecycle
docker ps
docker stop nginx-server
docker ps -a
docker rm nginx-server

## Skills Learned

I learned how to use basic Docker commands to pull images, run containers, check their status, stop them, and remove them. I also learned how port mapping allows a containerized application to be accessed through the host machine.

## Challenges Encountered

One challenge was remembering the correct Docker commands and understanding how the container port and host port are connected. Running the commands step by step helped me understand the Docker container lifecycle.
