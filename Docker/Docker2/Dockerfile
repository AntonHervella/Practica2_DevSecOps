FROM ubuntu:latest
WORKDIR /home/administrador/Practica2_DevSecOps/
RUN apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get install tzdata
RUN apt-get install apache2 git
EXPOSE 80
RUN apt-get install php
WORKDIR /var/www/html
RUN git clone https://github.com/drnic/php-helloworld.git
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
