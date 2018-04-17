cp ~/Downloads/docker_test.pem.txt ~/.ssh/docker_test.pem
chmod 400 ~/.ssh/docker_test.pem
ssh -i ~/.ssh/docker_test.pem ec2-user@INSERT_IP_HERE
