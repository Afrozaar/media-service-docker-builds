FROM openjdk:8-jre-slim
MAINTAINER "Michael Wiles <michael.wiles@afrozaar.com>"
VOLUME /tmp
# upgrade to EDGE
# NOTE: the use of exit 0; to ignore error during upgrade
#RUN cat /etc/apk/repositories

COPY etc/apt/preferences.d /etc/apt/preferences.d/
COPY etc/apt/sources.list.d /etc/apt/sources.list.d/

RUN apt-get update && apt-cache policy && apt-cache policy graphicsmagick && \
  apt-get install -y apt-utils  && apt-get upgrade -y  ; \
   apt-get install -y mediainfo ffmpeg youtube-dl webp libwebp-dev libxml2 exiftool graphicsmagick ghostscript file; exit 0; 
