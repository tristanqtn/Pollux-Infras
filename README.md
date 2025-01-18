# Pollux Infras

This repository contains everything to Pollux testing environment.

## Docker Containers

Docker containers are a good way to simulate a production environment. We provide you with the following docker containers to test Pollux:

- [Debian:latest](./docker/debian/Dockerfile): a Debian container with Python3 and Git installed.
- [Ubuntu:latest](./docker/ubuntu/Dockerfile): an Ubuntu container with Python3 and Git installed.
- [Windows:latest](./docker/windows/Dockerfile): a Windows container with Python3 and Git installed.
- [Fedora:latest](./docker/fedora/Dockerfile): a Fedora container with Python3 and Git installed.

### Build Docker Images

To build a docker image, you can use the following command in the correct path:

```bash
docker build -t <image_name> -f <Dockerfile_path> .
```

### Running Docker Containers

To run a docker container, you can use the following command:

```bash
docker run -it --name <container_name> <image_name>
```
