# XCA

![logo](https://assets.gitlab-static.net/uploads/-/system/project/avatar/17155228/xca.png)

- [XCA](#xca)
  - [INDEX](#index)
  - [BADGES](#badges)
  - [INTRODUCTION](#introduction)
  - [PREREQUISITES](#prerequisites)
  - [INSTALL](#install)
    - [DOCKER RUN](#docker-run)
    - [DOCKER COMPOSE](#docker-compose)
  - [LICENSE](#license)

## BADGES

[![pipeline status](https://gitlab.com/oda-alexandre/xca/badges/master/pipeline.svg)](https://gitlab.com/oda-alexandre/xca/commits/master)

## INTRODUCTION

Docker image of :

- [xca](https://hohnstaedt.de/xca)

Continuous integration on :

- [gitlab pipelines](https://gitlab.com/oda-alexandre/xca/pipelines)

Automatically updated on :

- [docker hub public](https://hub.docker.com/r/alexandreoda/xca)

## PREREQUISITES

Use [docker](https://www.docker.com)

## BUILD

### DOCKER RUN

```\
docker run -d --rm \
--name xca \
-e DISPLAY \
--env=QT_X11_NO_MITSHM=1 \
-v ${HOME}:/home/xca \
-v /tmp/.X11-unix/:/tmp/.X11-unix/ \
alexandreoda/xca
```

### DOCKER COMPOSE

```yml
version: "2.0"

services:
  xca:
    container_name: xca
    image: alexandreoda/xca
    restart: "no"
    privileged: false
    environment:
      - DISPLAY
      - QT_X11_NO_MITSHM=1
    volumes:
      - "${HOME}:/home/xca"
      - "/tmp/.X11-unix/:/tmp/.X11-unix/"
```

## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://gitlab.com/oda-alexandre/xca/blob/master/LICENSE)
