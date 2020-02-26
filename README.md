# XCA

<img src="https://assets.gitlab-static.net/uploads/-/system/project/avatar/17155228/xca.png" width="200" height="200"/>


## INDEX

- [XCA](#xca)
  - [INDEX](#index)
  - [BADGES](#badges)
  - [INTRODUCTION](#introduction)
  - [PREREQUISITES](#prerequisites)
  - [INSTALL](#install)
  - [LICENSE](#license)

## BADGES

[![pipeline status](https://gitlab.com/oda-alexandre/xca/badges/master/pipeline.svg)](https://gitlab.com/oda-alexandre/xca/commits/master)

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

```docker run -d --rm --name xca -v ${HOME}:/home/xca -v /tmp/.X11-unix/:/tmp/.X11-unix/ -e DISPLAY alexandreoda/xca```

## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://gitlab.com/oda-alexandre/xca/blob/master/LICENSE)
