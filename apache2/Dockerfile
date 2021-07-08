FROM ubuntu/apache2

RUN mkdir /code
WORKDIR /code

RUN sed -i "/\/var\/www\/html/c DocumentRoot \/var\/www\/html\/$SITE_NAME" /etc/apache2/sites-enabled/000-default.conf

RUN sed -i '/<Directory \/var\/www\/>/,/<\/Directory>/ s/AllowOverride None/AllowOverride All/' /etc/apache2/apache2.conf

RUN echo 'ServerName 127.0.0.1' >> /etc/apache2/sites-enabled/000-default.conf
