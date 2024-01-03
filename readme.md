build docker image

```bash
docker build -t <image_name> .
```

run docker container

```bash
docker run --name <container_name> -d -p 8080:8080 <image_name>
```

-d: run container in background and print container ID
-p: map port 8080 of the host to port 8080 in the container
--name: name of the container

stop docker container

```bash
docker stop <container_name>
```

list docker containers

```bash
docker ps
```

list all docker containers

```bash
docker ps -a
```

list docker images

```bash
docker images
```

start docker container

```bash
docker start <container_name>
```

remove docker container

```bash
docker rm <container_name>
```
