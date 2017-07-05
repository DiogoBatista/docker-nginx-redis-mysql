FROM webdevops/php-nginx:ubuntu-16.04

RUN apt update
RUN apt install -y nginx-extras

RUN touch /opt/docker/etc/supervisor.d/laravel.conf
ADD supervisor /opt/docker/etc/supervisor.d/laravel.conf

CMD ["supervisord"]