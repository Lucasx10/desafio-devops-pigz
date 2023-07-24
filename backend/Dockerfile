# Primeira imagem: PHP e Symfony
FROM php:8.0-fpm AS php

# Instalação das dependências do sistema
RUN apt update \
    && apt install -y zlib1g-dev g++ git libicu-dev zip libzip-dev zip libpq-dev \
    && apt clean

# Instalação das extensões do PHP
RUN docker-php-ext-install pdo pdo_pgsql intl opcache zip

# Instalação do Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Instalação do Symfony CLI diretamente no contêiner
RUN curl -sS https://get.symfony.com/cli/installer | bash
RUN mv /root/.symfony5/bin/symfony /usr/local/bin/symfony

# Criar um novo projeto Symfony em um diretório temporário
WORKDIR /var/www/app
RUN symfony new /var/www/app --no-interaction --no-git
