FROM mcr.microsoft.com/devcontainers/php:1-8.2-bookworm

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get install -y libicu-dev libonig-dev mariadb-client \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*
RUN docker-php-ext-install intl mbstring mysqli pdo pdo_mysql
