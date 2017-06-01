docker-lazarus
===========

Ubuntu based Docker environment for building Lazarus (FPC) applications.

[![Docker Hub](https://img.shields.io/badge/docker-ready-blue.svg)](https://registry.hub.docker.com/u/waleedsamy/docker-lazarus/)


## available compilers tags
 * `linux-amd64-1.6.4` or `latest`
 * `linux-i386-1.6.4`
 * `linux-amd64-1.2.6`
 * `linux-i386-1.2.6`
 * `linux-amd64-1.6.0`

## Starting the container:

```bash
docker run -it -v $PWD:/app -p 5901:5901 -w /app waleedsamy/docker-lazarus:latest /bin/bash
```


## Compiling

You can use the lazbuild:

```bash
lazbuild the-name-of-your-project.lpr

```


## Testing

If your application needs GUI, use vnc4server and connect to the container using a vnc client (port 5901):

```bash
vnc4server
```


## Credits

[@gabrielrcouto](http://www.twitter.com/gabrielrcouto)
