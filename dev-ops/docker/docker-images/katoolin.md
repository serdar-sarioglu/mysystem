## Katoolin Server

Katoolin is a KALI replika on ubunutu, this docker image runs as KALI

>From ubuntu

>MAINTAINER Serdar SARIOGLU <serdar.sarioglu@mysystem.org>

>RUN apt-get update && apt-get install -y git python

>RUN git clone https://github.com/LionSec/katoolin.git && cp katoolin/katoolin.py /usr/bin/katoolin

>RUN chmod +x /usr/bin/katoolin

>RUN sudo katoolin


## 

This Document has been written By Serdar Sarioglu - 2016

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=Visit%20mysystem.org"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate%20me-paypal-brightgreen.svg"></a>
