FROM frolvlad/alpine-oraclejdk8:slim
MAINTAINER "Johan Mynhardt <johan.mynhardt@gmail.com>"
VOLUME /tmp
# upgrade to EDGE
# NOTE: the use of exit 0; to ignore error during upgrade
RUN sed -i -e 's/v3\.7/edge/g' /etc/apk/repositories
#RUN cat /etc/apk/repositories
RUN apk upgrade --update-cache --available; exit 0;
RUN apk add ffmpeg youtube-dl libwebp libwebp-tools lcms2 tiff libjpeg libjpeg-turbo openjpeg libpng xz-libs libxml2 libgomp exiftool graphicsmagick ghostscript file; exit 0; 

