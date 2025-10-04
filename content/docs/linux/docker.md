---
title: "docker"
draft: false
---

# docker

## Docker System

```bash
docker system info
```

## Show hard disk usage

```bash
docker system df
```

## docker run

### Start a container from an image

```bash
docker run -it --rm <image>
```

### Override the entry point, e.g., with a shell to debug the container if the entry point is actually a binary

```bash
docker run --entrypoint "/bin/sh" -it --rm <image>
```

### Execute command in a temporary container, based on a specific image

```bash
docker run [options] <image> [command] [arguments]
```

## docker exec

### Execute a command in the container

```bash
docker exec [options] <container id or container name> <command>
```

## docker build

```bash
docker build -t hello-world .
```

### Overview of how many resources a container consumes

```bash
docker container stats -a --no-stream
```

### List users who have containers running

```bash
docker inspect $(docker ps -q) --format '{{.Config.User}} {{.Name}}'
```

## docker image

```bash
docker image prune -a
```

### Docker Logs Handling

```bash
docker logs <container name>  [optionen]
```

| Option |  Description |
| --- | --- |
| --details | Show extra information |
| --follow, -f | Follow |
| --since | Show logs since timestamp (e.g. 2013-01-02T13:23:37Z) or relative (e.g. 42m for 42 minutes) |
| --tail , -n | Number of lines to show from the end of the logs |
| --timestamps , -t | Show timestamps |
| --until | Show logs before a timestamp (e.g. 2013-01-02T13:23:37Z) or relative (e.g. 42m for 42 minutes) |

## docker volume

### List volumes

```bash
docker volume
```

### Copy file to volume

```bash
docker container create --name temp -v test_config:/data busybox
```

```bash
docker cp . temp:/data
```

```bash
docker rm temp
```

## docker events

### View docker events

```bash
docker events --since '18h'
```

```bash
docker stats --no-stream
```

## misc

Limit docker resources with docker compose

`https://docs.docker.com/compose/compose-file/compose-file-v3/#resources`
