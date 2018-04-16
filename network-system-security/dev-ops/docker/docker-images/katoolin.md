## Katoolin Server

Katoolin is a KALI replika on ubunutu, this docker image runs as KALI

>From ubuntu

>MAINTAINER Serdar SARIOGLU <serdar.sarioglu@mysystem.org>

>RUN apt-get update && apt-get install -y git python

>RUN git clone https://github.com/LionSec/katoolin.git && cp katoolin/katoolin.py /usr/bin/katoolin

>RUN chmod +x /usr/bin/katoolin

>RUN sudo katoolin


##
This Document has been written By Serdar Sarioglu - 2015

KeyWords: `DevOps` `Katoolin` `Docker` `Image`

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/badge/Visit-mysite-green.svg"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate-me-red.svg"></a>
<a href="mailto:serdar.sarioglu@mysystem.org" title="Email"><img src="https://img.shields.io/badge/Email-me-blue.svg"></a>
<a href="https://www.linkedin.com/in/serdarsarioglu/" title="Linkedin"><img src="https://img.shields.io/badge/Linkedin-me-orange.svg"></a>
