FROM php:7.4-apache

# tzdata install
RUN apt-get update && apt-get install -y \
    tzdata \
    libpq-dev \
 && rm -rf /var/lib/apt/lists/* \
 && docker-php-ext-install pdo_pgsql

# set timezone
ENV TZ=Asia/Tokyo

