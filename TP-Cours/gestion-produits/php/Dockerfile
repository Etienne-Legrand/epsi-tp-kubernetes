FROM php:8.0-apache
# Activer les extensions pour mysql
RUN docker-php-ext-install mysqli pdo pdo_mysql
# Copier les fichiers de l'app vers /var/www/html
COPY ./www /var/www/html
# Donner accès en lecture/écriture au dossier uploads
RUN chmod -R 777 /var/www/html/uploads