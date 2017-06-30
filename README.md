# PHP 7.1 with nginx
> Sandbox for development

[![CircleCI](https://img.shields.io/circleci/project/dockerphp/7.1-nginx/release.svg)](https://circleci.com/gh/dockerphp/7.1-nginx)
[![Docker Stars](https://img.shields.io/docker/stars/dockerphp/7.1-nginx.svg)][hub]
[![Docker Pulls](https://img.shields.io/docker/pulls/dockerphp/7.1-nginx.svg)][hub]

Includes the following dependencies:
- NodeJs
- Sass
- Yarn
- Composer

## Installation
Pull the image from the docker index rather than downloading the git repo. This prevents you having to build the image on every docker host.

    docker pull dockerphp/7.1-nginx 

## Running

To simply run the container:

    $ docker run -d -p 80:80 dockerphp/7.1-nginx --name nginx

## Volumes

If you want to link to your web site directory on the docker host to the container run:

    $ docker run -d -p 80:80 dockerphp/7.1-nginx  -v /your/project:/app

## Enabling SSL

    $ docker run -d -p 80:80 -p 443:443 -v your_crt_key_files:/etc/ssl/nginx/

## Run console mode

    docker run -p 80:80 -a stdin -a stdout -i -t dockerphp/7.1-nginx /bin/bash

##  License

The code in this repository, unless otherwise noted, is MIT licensed. See the LICENSE file in this repository.

[hub]: https://hub.docker.com/r/dockerphp/7.1-nginx/
