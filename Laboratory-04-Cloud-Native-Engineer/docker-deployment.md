### 1. List Running Containers

```bash
docker ps
```

This command displays the containers that are currently running.

### 2. Stop the Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### 3. Verify the Container is Stopped

```bash
docker ps
docker ps -a
```

These commands verify that the Nginx container is no longer running and can still be viewed among stopped containers.

### 4. Remove the Container

```bash
docker rm nginx-server
```

This command permanently removes the stopped Nginx container from the Docker environment.

## Nginx Deployment

The official Nginx image was downloaded using:

```bash
docker pull nginx
```

The container was started in detached mode using:

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

The web server was tested using:

```bash
curl http://localhost:8080
```

Port `8080` on the host was mapped to port `80` inside the Nginx container so that the web server could be accessed through the host machine.

## Evidence

The terminal screenshot showing the container lifecycle commands is stored in:

`screenshots/container-lifecycle.png`

