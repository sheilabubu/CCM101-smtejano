# Container Observability

## Overview

In this laboratory activity, I learned how to deploy a web server using Docker, send HTTP requests, check application logs, and monitor container resources. These tasks helped me understand how a Cloud Operations Engineer checks whether a web application is running properly.

## Nginx Container Deployment

I created a Docker container named `clientwebsite` using the Nginx image. I ran the container in the background and mapped port 8080 on the host to port 80 inside the container so that I could access the website.

The command used was:

```bash
docker run -d --name clientwebsite -p 8080:80 nginx
```

I used `docker ps` to check that the container was running.

## HTTP Traffic Generation

I used the `curl` command to send three HTTP requests to the Nginx website.

```bash
curl http://localhost:8080
```

All three requests returned the default Nginx welcome page with an HTTP 200 status code, showing that the web server was responding successfully.

I also requested a page that does not exist by running:

```bash
curl http://localhost:8080/hidden-admin-page
```

The server returned a 404 Not Found response because the requested page was unavailable.

## Application Logging

### 404 Error Log

The following log entry was recorded when I requested the nonexistent page:

```text
172.17.0.1 - - [11/Oct/2026:11:15:49 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0"
```

### Importance of Application Logs

Application logs help administrators understand how a web server behaves by recording incoming requests and their responses. When an error occurs, these records provide useful details that help locate the problem and make troubleshooting easier.

## Real-Time Container Metrics

### Docker Resource Monitoring

I used the `docker stats` command to monitor the resource consumption of the `clientwebsite` container. It displayed the CPU usage, memory consumption, network activity, and block input/output in real time.

### Recorded Metrics

- **Container Name:** `clientwebsite`
- **CPU Usage:** 0.00%
- **Memory Usage:** 2.793 MiB
- **Memory Limit:** 1.859 GiB
- **Memory Usage Percentage:** 0.15%
- **Network I/O:** 4.58 kB / 6.89 kB
- **Block I/O:** 49.2 kB / 12.3 kB
- **PIDs:** 2

### Observation

The container was using 0.00% CPU and 2.793 MiB of memory when I captured the screenshot. This indicates that the container was consuming very little CPU and memory at that moment, although its resource usage may increase when it receives more traffic.

