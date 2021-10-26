# Web SSH Docker

nginx container with ssh. You can login to the container and update the website.

## Build

```shell
docker build -t nginx-ssh .
```

## Usage

```shell
docker run -itd -p YOUR_SSH_PORT:22 -p YOUR_WEB_PORT:80 -e NAME=YOUR_USER_NAME -e PASSWORD=YOUR_PASSWORD --name YOUR_CONTAINER_NAME nginx-ssh
```