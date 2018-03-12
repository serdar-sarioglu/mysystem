## Web Server on Ubuntu
>From ubuntu

>MAINTAINER Serdar SARIOGLU <serdar.sarioglu@mysystem.org>

>RUN apt-get update && apt-get install -y apache2 php libapache2-mod-php mariadb-server mariadb-client php-mbstring php-xmlrpc php-soap php-gd php-xml php-intl php-mysql php-cli php-mcrypt php-ldap php-zip php-curl php7.0-mysql php7.0-curl php7.0-gd php7.0-intl php-pear php-imagick php7.0-imap php7.0-mcrypt php-memcache  php7.0-pspell php7.0-recode php7.0-sqlite3 php7.0-tidy php7.0-xmlrpc php7.0-xsl php7.0-mbstring php-gettext

>RUN /etc/init.d/apache2 start && /etc/init.d/mysql start

>CMD ["echo", "Services are up and running!"]

> EXPOSE 80



##
This Document has been written By Serdar Sarioglu - 2015

KeyWords: `WebServer` `Docker` `Ubuntu`

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/badge/Visit-mysite-green.svg"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate-me-red.svg"></a>
<a href="mailto:serdar.sarioglu@mysystem.org" title="Email"><img src="https://img.shields.io/badge/Email-me-blue.svg"></a>
<a href="https://www.linkedin.com/in/serdarsarioglu/" title="Linkedin"><img src="https://img.shields.io/badge/Linkedin-me-orange.svg"></a>
