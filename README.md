# XCA

![logo](https://assets.gitlab-static.net/uploads/-/system/project/avatar/17155228/xca.png)

## INDEX

- [XCA](#xca)
  - [INDEX](#index)
  - [BADGES](#badges)
  - [FIRST UPDATE](#first-update)
  - [INTRODUCTION](#introduction)
  - [PREREQUISITES](#prerequisites)
  - [INSTALL](#install)
  - [LICENSE](#license)

## BADGES

[![pipeline status](https://gitlab.com/oda-alexandre/xca/badges/master/pipeline.svg)](https://gitlab.com/oda-alexandre/xca/commits/master)

## FIRST UPDATE

Date: 01-01-01

## INTRODUCTION

Docker image of :

- [xca](https://hohnstaedt.de/xca)

Continuous integration on :

- [gitlab](https://gitlab.com/oda-alexandre/xca/pipelines)

Automatically updated on :

- [docker hub public](https://hub.docker.com/r/alexandreoda/xca)

## PREREQUISITES

Use [docker](https://www.docker.com)

## INSTALL

```docker run -d --rm --name xca -v ${HOME}:/home/xca -v /tmp/.X11-unix/:/tmp/.X11-unix/ --env=QT_X11_NO_MITSHM=1 -e DISPLAY alexandreoda/xca```

## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://gitlab.com/oda-alexandre/xca/blob/master/LICENSE)