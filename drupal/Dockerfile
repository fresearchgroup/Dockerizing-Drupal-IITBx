FROM drupal:9.2.0-php7.4-fpm-alpine3.13

RUN mkdir /code
WORKDIR /code

#ENV USER=root

RUN cd /opt/drupal/web/sites/default \
    && cp default.settings.php settings.php \
    && cp default.services.yml services.yml \
    && chmod a+w settings.php \ 
    && chmod a+w services.yml 


