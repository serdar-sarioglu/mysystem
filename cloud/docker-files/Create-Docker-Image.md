## Create Docker Image

We will create a test web server contains mariadb.

First create a file with your text editor:
>mkdir sample-web-server

>vi dockerfile

You will need a base image from dockerhub https://hub.docker.com and use sample CMD 

>From ubuntu

>CMD ["echo", "hello world!"]

>RUN apt-get update && apt-get install -y apache2 php libapache2-mod-php mariadb-server mariadb-client libapache2-mod-php-common php-mbstring php-xmlrpc php-soap php-gd php-xml php-intl php-mysql php-cli php-mcrypt php-ldap php-zip php-curl

>RUN systemctl enable apache2.service mariadb.service

>RUN systemctl start apache2.service mariadb.service



#### How to build the image:
>docker build .

#### How to run the image:
>docker run --name test docker_image_id
## 

This Document has been written By Serdar Sarioglu - 2016

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=Visit%20mysystem.org"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate%20me-paypal-brightgreen.svg"></a>
