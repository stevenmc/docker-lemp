docker-lemp
===========

Docker environment for LEMP development work.  Not intended for production.

Do not use it in production environment.

# Usage

    docker run -d --name=lemp \
      -v /var/www/project-name/:/var/www/ \
      -v /var/lib/mysql:/var/lib/mysql \
      -p 8008:80 \
      -t project-name \
      stevenmc/docker-lemp:latest

# Detail

## MySQL
* user: root
* (No password)

## SSH
SSH not supported. You can use `docker exec` to enter the docker container.
