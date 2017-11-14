# Nginx

This is a minimal docker container based on alphine. It also has lets encrypt pre installed to automatically secure https content.

## What is supported

Supported tags and respective Dockerfile links
3.6, latest (3.6/Dockerfile)

 Supported architectures: (more info)
amd64, arm32v7 ( Raspberry PI 2) , arm64v8 ( Raspberry PI 3), i386, ppc64le, s390x)


## How to use this container

### Basic Usage

```bash

docker run --name nginx -p 80:80 -p 443:443 libertaria/nginx:armv7

```

### Mounting volumes

The container serves content from inside /usr/html/ by default on the localhost. It checks for index.html file . If you would like to modify this point the container volume to the voume on your device.

```bash

docker run --name nginx -p 80:80 -p 443:443  -v my/device/folder:/usr/html libertaria/nginx:armv7

```
 

