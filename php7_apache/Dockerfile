FROM php:7.0-apache
# Install modules
RUN apt-get update && apt-get install -y libpq-dev libicu-dev && docker-php-ext-install pdo pdo_pgsql pgsql intl

# Habilitar Mod_reqwite do Apache2
RUN a2enmod rewrite

RUN apt-get autoclean && apt-get autoremove && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*