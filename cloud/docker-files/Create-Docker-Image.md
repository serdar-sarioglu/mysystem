## Create Docker Image

First create a file with your text editor:
>vi my-docker

You will need a base image from dockerhub https://hub.docker.com and use sample CMD 

>From ubuntu

>CMD ["echo", "hello world!"]

#### Run a script in Docker Image
Firsty create a bash script  run.sh like;

>#! /bin/sh

>echo hello world!


On Docker file (my-docker);

>From ubuntu

>COPY run.sh /run.sh


#### How to build the image:
>docker build my-docker

#### How to run the image:
>docker run --name test docker_image_id
## 

This Document has been written By Serdar Sarioglu - 2016

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=Visit%20mysystem.org"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate%20me-paypal-brightgreen.svg"></a>
