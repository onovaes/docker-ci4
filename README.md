# Docker and Codeigniter 4

Nginx 1.17.8 + PHP 7.4-fpm + CodeIgniter 4.0.4 -> http://localhost:8080

## Installing

    $git clone git@github.com:onovaes/docker-ci4.git

    $cd docker-ci4 

    $cp docker/env-example .env

    $docker-compose up -d

    $docker exec -ti php_app composer update