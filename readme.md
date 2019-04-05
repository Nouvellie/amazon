###### ######
# AMAZON
###### ######

## Use ##

A new dynamic ip is generated, it is accessed from ssh more easily. (can be static)
IP (IPv4 Public IP) --> 000.000.000.000

## Create a security group ##
This one can be used in any instance.
* Inbound:
HTTP  -->  TCP  -->  80  --> IP
SSH   -->  TCP  -->  22  --> IP
MYSQL -->  TCP  --> 3306 --> IP
* Outbound:
All traffic.

## SSH ## 
ssh -i ~path/file.pem user@000.000.000.000
* Chmod the key:
sudo chmod 400 file.pem
* Are you sure you want to continue connecting (ECDSA key fingerprint)
yes