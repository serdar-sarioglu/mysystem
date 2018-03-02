>From centos

>MAINTAINER Serdar SARIOGLU <serdar.sarioglu@mysystem.org>

>RUN yum update && yum install glibc.i686 libstdc++.i686 wget -y

>RUN wget https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz

>RUN tar xf steamcmd_linux.tar.gz

>RUN ./steamcmd.sh +login anonymous +force_install_dir force_install_dir /root/csgo +app_update 740 validate +quit

>CMD ["echo", "CS Server installed succesfully!"]

>EXPOSE 80