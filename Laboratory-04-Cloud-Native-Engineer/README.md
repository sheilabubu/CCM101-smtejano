# Mission Overview

This mission introduced me to the basics of cloud-native engineering and Docker containerization. I learned how containers work and how they are different from traditional Virtual Machines (VMs). The activities were completed using the KillerCoda Playground, where I practiced deploying an Nginx web server, checking the Docker environment, and managing a container from start to finish.

## Objectives

* Differentiate between Virtual Machines (VMs) and containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Practice using basic Docker CLI commands.
* Download and run an Nginx Docker image.
* Check if the Nginx web server is working properly.
* Perform basic container lifecycle operations.
* Record Docker activities using Markdown.

## Docker Commands Executed

### Docker Verification

```bash
docker --version
```

```bash
docker info
```

### Nginx Deployment

```bash
docker pull nginx
```

```bash
docker run -d -p 8080:80 nginx
```

```bash
curl http://localhost:8080
```

### Container Lifecycle

```bash
docker ps
```

```bash
docker stop <CONTAINER_ID>
```

```bash
docker ps -a
```

```bash
docker rm <CONTAINER_ID>
```

```bash
docker ps -a
```

## Skills Learned

In this laboratory activity, I gained an experience with Docker and learned how containers can be used to run applications in a cloud environment. I practiced using Docker commands to download images, create containers, check their status, and remove them when they were no longer needed. I also learned how port mapping works and used `curl` to check the Nginx web server. Aside from Docker, I also improved my ability to organize technical information and document my work using Markdown and GitHub.

## Challenges Encountered

I found some Docker commands confusing because I was still learning what each command does and when it should be used. I also had to understand how the container ID is used when stopping and removing a container. Another challenge was making sure that the commands were executed in the correct sequence, especially during the container lifecycle activity. By following the instructions and checking the output after each command, I was able to understand the process better and complete the activity successfully.

