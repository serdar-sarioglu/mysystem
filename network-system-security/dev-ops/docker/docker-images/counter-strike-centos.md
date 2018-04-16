## Counter Strike Server On Centos

Docker image contains counterstrike server, just run! Have Fun LoL

>From centos

>MAINTAINER Serdar SARIOGLU <serdar.sarioglu@mysystem.org>

>RUN yum update 

>RUN yum install glibc.i686 libstdc++.i686 wget -y

>RUN wget https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz

>RUN tar xf steamcmd_linux.tar.gz

>RUN ./steamcmd.sh +login anonymous +force_install_dir force_install_dir ../csgo +app_update 740 validate +quit

>CMD ["echo", "CS Server installed succesfully!"]

>EXPOSE 27015


##
This Document has been written By Serdar Sarioglu - 2015

KeyWords: `Counter` `Strike` `Docker` `Image`

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/badge/Visit-mysite-green.svg"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate-me-red.svg"></a>
<a href="mailto:serdar.sarioglu@mysystem.org" title="Email"><img src="https://img.shields.io/badge/Email-me-blue.svg"></a>
<a href="https://www.linkedin.com/in/serdarsarioglu/" title="Linkedin"><img src="https://img.shields.io/badge/Linkedin-me-orange.svg"></a>
