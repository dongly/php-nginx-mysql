FROM php:fpm-alpine

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.ustc.edu.cn/g' /etc/apk/repositories && \
	apk add --no-cache --update \
	libxml2 libxml2-dev && \
	docker-php-ext-install mysqli soap && \
	docker-php-ext-enable mysqli soap
