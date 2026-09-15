# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory introduces cloud-native engineering concepts by comparing traditional Virtual Machines with containers and demonstrating the deployment and management of a Docker container. An Nginx web server was deployed using Docker and accessed through a mapped network port.

## Objectives

* Differentiate Virtual Machines and containers.
* Verify that Docker is installed and running.
* Pull and run a Docker image.
* Deploy an Nginx web server in a container.
* Map a host port to a container port.
* Manage the container lifecycle.
* Document Docker operations using Markdown.

## Docker Commands Executed

### Docker Verification

```bash
docker --version
docker info
```

### Nginx Deployment

```bash
docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
curl http://localhost:8080
```

### Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

## Skills Learned

* Docker command-line operations
* Container deployment
* Nginx deployment
* Port mapping
* Container lifecycle management
* Linux terminal usage
* Technical documentation using Markdown
* GitHub repository organization

## Challenges Encountered

One challenge was becoming familiar with Docker commands and understanding the difference between an image and a running container. Another challenge was understanding port mapping and how port `8080` on the host connects to port `80` inside the Nginx container. The KillerCoda environment helped provide a practical environment for testing these concepts.
