FROM php:8.5.0RC2-trixie

RUN curl -LSs https://box-project.github.io/box2/installer.php | php
RUN mv /box.phar /usr/local/bin/box

RUN echo "phar.readonly = off" > /usr/local/etc/php/php.ini

WORKDIR /source

ENTRYPOINT ["/usr/local/bin/box"]
CMD [""]
