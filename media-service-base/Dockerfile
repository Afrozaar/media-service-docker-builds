FROM afrozaar/alpinegm-java
# We're using a custom alpinegm build as the standard graphicsmagick package
#   is not fully functional.

MAINTAINER "Johan Mynhardt <johanmynhardt@gmail.com>"
VOLUME /tmp

RUN apk update
RUN apk add exiftool ghostscript file

