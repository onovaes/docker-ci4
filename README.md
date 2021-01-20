# Docker and Codeigniter 4 

DEVELOPMENT Environment for CodeIgniter 4 with Docker

Nginx 1.17.8 + PHP 7.4-fpm + CodeIgniter 4.0.4 -> http://localhost:8080


## Cloning

    $git clone git@github.com:onovaes/docker-ci4.git my_project

    $cd my_project 


## Configuring (http://localhost:8080/)

    $cp docker/env-example .env


## Running Containers

    $docker-compose up 


## Installing Lastest Code Igniter and Dependencies

    $docker exec -ti ci4_php_app composer install


## Running Tests

    $docker exec -ti ci4_php_app composer test
