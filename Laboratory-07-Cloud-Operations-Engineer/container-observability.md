# Container Observability

## Objective

The purpose of this activity is to deploy an Nginx web server using Docker and generate HTTP traffic to observe how the application responds to requests.

## Container Deployment

I deployed an Nginx container named `clientwebsite` and mapped port 8080 on the host to port 80 inside the container.

## Traffic Generation

I sent three HTTP requests using the `curl` command to test whether the website was accessible. The requests returned the default Nginx welcome page.

## Error Testing

I requested `/hidden-admin-page` to test how the web server handles a nonexistent page. The server returned a 404 Not Found response because the requested page was unavailable.


