docker-lazarus
===========

Debian based Docker environment for building Lazarus (FPC) applications.


## Starting the container:

```bash
docker run -it -v $PWD:/app -p 5901:5901 -w /app gabrielrcouto/docker-lazarus:latest /bin/bash
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