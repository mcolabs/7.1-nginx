# NGINX PHP 7.1

> Sandbox Nginx PHP 7.1

![enter image description here](https://circleci.com/gh/registry-docker/nginx-php-7.1.png?circle-token=:circle-token)

Build image:
---------------

    docker build -t "registry-docker/nginx-php-7.1" . 

Run
---------------

    docker run -d -p 80:80 registry-docker/nginx-php-7.1  -v /your/project:/app

Run console mode
---------------

    docker run -p 80:80 -a stdin -a stdout -i -t registry-docker/nginx-php-7.1  /bin/bash


## License

Copyright &copy; 2016 [Michael COULLERET aka 20uf](http://github.com/20uf). Licensed under the terms of the [MIT license](LICENSE.md).
