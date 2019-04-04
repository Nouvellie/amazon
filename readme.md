###### ######
# NOUVELLIE
###### ######

# LAUNCH INSTANCE EC2 - UBUNTU (18.04 LTS)

## Choose instance ##
T1, T2, T3, etc.

## Configure instance ##
Number of instances, network, subnet, placement group, etc.

## Add storage ##
Hdd/sdd settings, delete on termination checkbox.

## Tags ##
Keys*

## Security groups ##
New or existing.


# LAUNCH #

# SELECT AN EXISTING KEY PAIR OR CREATE A NEW ONE
* If create:
Create a key pair name and then download it.

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