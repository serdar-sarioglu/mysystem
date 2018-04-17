## Docker Samples

#### Run MySQL
>docker run --name db -e MYSQL_ROOT_PASSWORD="mypass" -d mysql/mysql-server:5.5

#### Run WordPress
>docker run --name wordpress-1 --link db:mysql -e WORDPRESS_DB_NAME="wordpress_1" -d -p 80:80 wordpress:latest

## 

This Document has been written By Serdar Sarioglu - 2016

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=Visit%20mysystem.org"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate%20me-paypal-brightgreen.svg"></a>
