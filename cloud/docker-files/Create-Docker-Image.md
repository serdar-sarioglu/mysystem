## Create Docker Image

We will create a test web server contains mariadb.

First create a file with your text editor:
>mkdir sample-web-server

>vi dockerfile

You will need a base image from dockerhub https://hub.docker.com and use sample CMD 

>From ubuntu

>CMD ["echo", "Staring Installation!"]

>RUN apt-get update && apt-get install -y apache2 php libapache2-mod-php mariadb-server mariadb-client php-mbstring php-xmlrpc php-soap php-gd php-xml php-intl php-mysql php-cli php-mcrypt php-ldap php-zip php-curl php7.0-mysql php7.0-curl php7.0-gd php7.0-intl php-pear php-imagick php7.0-imap php7.0-mcrypt php-memcache  php7.0-pspell php7.0-recode php7.0-sqlite3 php7.0-tidy php7.0-xmlrpc php7.0-xsl php7.0-mbstring php-gettext

>CMD ["echo", "Requiremets installed suceesfully"]

>RUN systemctl start apache2.service mysql.service

>CMD ["echo", "Services are up and running!"]


#### How to build the image:
>docker build .

#### How to run the image:
>docker run --name test docker_image_id
## 

This Document has been written By Serdar Sarioglu - 2016

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=Visit%20mysystem.org"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate%20me-paypal-brightgreen.svg"></a>
