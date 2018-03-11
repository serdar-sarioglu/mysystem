install-webmin-centos.md


*Run as root

wget http://prdownloads.sourceforge.net/webadmin/webmin-1.870-1.noarch.rpm
yum -y install perl perl-Net-SSLeay openssl perl-IO-Tty perl-Encode-Detect
rpm -U webmin-1.870-1.noarch.rpm
systemctl enable webmin
