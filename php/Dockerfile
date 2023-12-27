FROM php:8.2-apache


RUN apt-get update && apt-get install -y \
    zlib1g-dev \
    libzip-dev \
    unzip \
    curl

RUN docker-php-ext-install pdo_mysql

RUN docker-php-ext-install zip

RUN service apache2 restart

WORKDIR /var/www/html/steko_id

#COPY ./apache/steko-id.conf /etc/apache2/sites-available/


#RUN ln -s /etc/apache2/sites-available/steko-id.conf /etc/apache2/sites-enabled/steko-id.conf

#RUN a2ensite steko-id.conf

#RUN  service apache2 restart


#RUN chown -R www-data:www-data ./storage/

#CMD chown -R www-data:www-data storage

#RUN find /var/www/html/steko_id -type d -exec chmod 0770 {} \;
#RUN find /var/www/html/steko_id -type f -exec chmod 0660 {} \;


#RUN chmod -R 750 /var/www/html/steko_id/storage/
