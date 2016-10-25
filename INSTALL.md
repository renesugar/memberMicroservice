# Installation 


# 1. Installation via Docker Images

This instruction provides a simple way to incorporate chamaconekt-members  into your private infrastructure 
through Docker Images.

This image provides a default, non-validating, ephemeral configuration that should work for most developers.
By configuring a container using this image with a host-based volume an operator gains access to full configuration, 
customization and persistance of data.


## Running locally

Build and run using Docker Compose:

```bash
$ git clone https://github.com/chamaconekt/members
```

```bash
$ cd members
```

```bash
$ docker-compose-up
```

## Deploying to Docker Cloud

[![Deploy to Docker Cloud](https://files.cloud.docker.com/images/deploy-to-dockercloud.svg)](https://cloud.docker.com/stack/deploy/)

Docker Cloud makes it easy for new Docker users to build and deploy their applications.Docker Cloud's operations
interface empowers seasoned Docker users to manage a full spectrum of applications, from single container apps to
distributed microservice stacks,anywhere.

Install the [Docker Cloud client](https://docs.docker.com/docker-cloud/installing-cli/)

```bash
$ docker login
```

```bash
$ docker-cloud stack up
```

## Docker Pull Command

```bash
$ docker pull chamaconektkenya/members
```


## What happens under the hood?

Docker client contacts the Docker Daemon.
Docker daemon pulls the "chamaconektkenya/members" image from Docker Hub
Docker daemon creates a new container from the "chamaconektkenya/members" image.

## How is this image created?

This image is created via this [Dockerfile]().


## Supported Docker versions

This image is officially supported on Docker version 1.12.2

Support for older versions (down to 1.6) is provided on a best-effort basis

Please see the Docker installation documentation for details on how to upgrade your Docker daemon







