# media-service-docker-builds
Docker builds for media-service (to build images that media-service depends on)

Build the docker image and tag it latest:
```
$ docker build -t afrozaar/ubuntu-gm:latest .
```
Check your image is available:
```
$ docker images
```
Push the new image to dockerhub:
```
$ docker push afrozaar/ubuntu-gm
```
The dependencies have been streamlined, so now only afrozaar/alpinegm2 is used.

UPDATE: we now use ubuntu-gm as alpine builds of graphics magick do not included support for webp format

