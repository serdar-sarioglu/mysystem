This Document has been written By Serdar Sarioglu - 2016
Serdar.Sarioglu@mysystem.org

######Login a custom registry:######
docker login registry.mysystem.org

######List images######
docker images --all

######Make image local######
docker save -o <save image to path> <image name>
docker save -o /home/mysystem/ftp-server-1 ftp-server-1

######Export local image######
docker load -i <path to image tar file>

######Bonus (Copy file with SCP)######
scp serdar@10.10.10.100:/home/mysystem/ftp-server-1 /root/images


