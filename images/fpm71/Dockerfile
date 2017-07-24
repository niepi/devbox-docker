FROM exozet/php-fpm:7.1.3
WORKDIR /var/www
RUN apt-get update -y \
  && apt-get install -y \
    libxml2-dev \
    php-soap \
  && apt-get clean -y
RUN docker-php-ext-install soap
RUN docker-php-ext-install zip