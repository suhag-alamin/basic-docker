build docker image

```bash
docker build -t <image_name> .
```

-t: name and optionally a tag in the 'name:tag' format

build docker image with tag

```bash
docker build -t <image_name>:<tag> .
```

run docker container

```bash
docker run --name <container_name> -d -p 8080:8080 <image_name>
```

run container with specific tag

```bash
docker run --name <container_name> -d -p 8080:8080 <image_name>:<tag>
```

run container with specific tag and environment variable

```bash
docker run --name <container_name> -d -p 8080:8080 -e <env_variable>=<value> <image_name>:<tag>
```

run container with specific tag and environment variable and volume

```bash'
docker run --name <container_name> -d -p 8080:8080 -e <env_variable>=<value> -v <host_path>:<container_path> <image_name>:<tag>
```

run container and remove it after exit

```bash
docker run --rm --name <container_name> -d -p 8080:8080 <image_name>
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
or
docker container rm <container_name>

```

remove docker image

```bash
docker rmi <image_name>
or
docker image rm <image_name>
```

remove everything

```bash
docker system prune -a
```
