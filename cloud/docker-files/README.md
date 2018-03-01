## Docker Commands

#### Login a custom registry:
>docker login registry.mysystem.org

#### List Images:
>docker images --all

#### List Containers:
>docker ps

#### Run a Docker Image:
>docker run --name test container_id

#### Remove Docker Container
>docker rm test

#### Remove Image:
>docker rmi image_name

#### Export Image:
>docker save -o save-image-to-path image-name

>docker save -o /home/mysystem/ftp-server-1 ftp-server-1

#### Import Image:
>docker load -i path-to-image-tar-file

#### Bonus (Copy file with SCP):
>scp serdar@10.10.10.100:/home/mysystem/ftp-server-1 /root/images

## 

This Document has been written By Serdar Sarioglu - 2016

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=Visit%20mysystem.org"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate%20me-paypal-brightgreen.svg"></a>
