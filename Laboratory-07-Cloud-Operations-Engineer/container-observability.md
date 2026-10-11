# Container Observability

## Objective

The purpose of this activity is to deploy an Nginx web server using Docker and generate HTTP traffic to observe how the application responds to requests.

## Container Deployment

I deployed an Nginx container named `clientwebsite` and mapped port 8080 on the host to port 80 inside the container.

## Traffic Generation

I sent three HTTP requests using the `curl` command to test whether the website was accessible. The requests returned the default Nginx welcome page.

## Error Testing

I requested `/hidden-admin-page` to test how the web server handles a nonexistent page. The server returned a 404 Not Found response because the requested page was unavailable.

## Application Log Analysis

### 404 Error Log

```text
172.17.0.1 - - [11/Oct/2026:11:15:49 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0"
```

### Importance of Application Logs

Application logs are important because they show the requests received by the web server and help identify errors when users try to access the website. They make troubleshooting easier by providing information about what happened, allowing the administrator to investigate the problem and find an appropriate solution.

