# Docker Deployment

## Deploying an Nginx Web Server

### 1. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub.

### 2. Run the Nginx Container

```bash
docker run -d -p 8080:80 nginx
```

This command runs the Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

### 3. Verify the Nginx Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx server and displays the HTML code of the Nginx welcome page.

The successful response should contain:

```text
Welcome to nginx!
```

## Container Lifecycle

### 1. List Running Containers

```bash
docker ps
```

This command lists all currently running Docker containers and displays information such as the container ID, image, status, and port mapping.

### 2. Stop the Running Container

```bash
docker stop <CONTAINER_ID>
```

This command stops the running Nginx container using its container ID.

### 3. Verify the Container is Stopped

```bash
docker ps -a
```

This command lists all containers, including stopped containers, to verify that the Nginx container has an exited status.

### 4. Remove the Container Completely

```bash
docker rm <CONTAINER_ID>
```

This command removes the stopped Nginx container completely from the Docker environment.

### 5. Verify the Container was Removed

```bash
docker ps -a
```

This command confirms that the Nginx container no longer appears in the list of containers.
