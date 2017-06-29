# dockerphp 7.1 nginx

[![CircleCI](https://img.shields.io/circleci/project/dockerphp/7.1-nginx/release.svg)](https://circleci.com/gh/dockerphp/7.1-nginx)
[![Docker Stars](https://img.shields.io/docker/stars/dockerphp/7.1-nginx.svg)][hub]
[![Docker Pulls](https://img.shields.io/docker/pulls/dockerphp/7.1-nginx.svg)][hub]

A super small Docker image based on [Ubuntu Linux][ubuntu].

##  Build image:

    docker build -t "dockerphp/7.1-nginx" . 

## Run

    docker run -d -p 80:80 dockerphp/7.1-nginx  -v /your/project:/app

## Run console mode

    docker run -p 80:80 -a stdin -a stdout -i -t dockerphp/7.1-nginx /bin/bash

##  License

The code in this repository, unless otherwise noted, is MIT licensed. See the LICENSE file in this repository.

[hub]: https://hub.docker.com/r/dockerphp/7.1-nginx/
