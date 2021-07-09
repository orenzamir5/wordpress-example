FROM wordpress:latest

RUN apt update && \
    apt install -y curl

WORKDIR /var/www/html/

ADD wordpress.tar.gz /var/www/