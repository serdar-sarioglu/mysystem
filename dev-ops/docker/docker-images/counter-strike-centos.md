## Counter Strike Server On Centos

Docker image contains counterstrike server, just run! Have Fun LoL

>From centos

>MAINTAINER Serdar SARIOGLU <serdar.sarioglu@mysystem.org>

>RUN yum update 

>RUN yum install glibc.i686 libstdc++.i686 wget -y

>RUN wget https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz

>RUN tar xf steamcmd_linux.tar.gz

>RUN ./steamcmd.sh +login anonymous +force_install_dir force_install_dir /root/csgo +app_update 740 validate +quit

>CMD ["echo", "CS Server installed succesfully!"]

>EXPOSE 80


## 

This Document has been written By Serdar Sarioglu - 2016

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=Visit%20mysystem.org"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate%20me-paypal-brightgreen.svg"></a>
