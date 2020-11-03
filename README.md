# Docker and Codeigniter 4

Only Nginx 1.17.8 -> http://localhost

Nginx 1.17.8 + PHP 7.4-fpm + CodeIgniter 4.0.4 -> http://app.localhost

## Installing

    $git clone git@github.com:onovaes/docker-ci4.git

    $cd docker-ci4

    $docker-compose up -d

    $docker exec -ti php_app composer update