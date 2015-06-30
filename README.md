docker-lemp
===========

Docker environment for LEMP development work.  Not intended for production.

Do not use it in production environment.

# Usage

	docker build -t cakephp-lemp .

docker run -d --name=lemp \
  -v /var/www/project-dir/:/var/www/ \
  -v /var/lib/mysql:/var/lib/mysql \
  -p 8008:80 \
  -t cakephp-lemp 

# Detail

## MySQL
* user: root
* (No password)

## SSH
SSH not supported. You can use `docker exec` to enter the docker container.
