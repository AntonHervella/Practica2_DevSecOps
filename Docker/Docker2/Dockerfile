FROM ubuntu:latest
WORKDIR /home
RUN apt-get update -y
RUN DEBIAN_FRONTEND=noninteractive apt-get install -y tzdata
RUN apt-get install -y apache2 git
EXPOSE 80
WORKDIR /var/www/html
RUN git clone https://github.com/drnic/php-helloworld.git
RUN apt-get install -y php
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
