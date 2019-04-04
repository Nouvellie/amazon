###### ######
## NOUVELLIE ##
###### ######

# LAUNCH INSTANCE EC2

## Choose Instance ##
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

# Select an existing key pair or create a new key pair
* If create:
Create a key pair name and then download it.

## USE ##

A new dynamic ip is generated, it is accessed from ssh more easily.
IP (IPv4 Public IP) --> 000.000.000.000

## Create a security group ##
This one can be used in any instance.
* Inbound:
HTTP  -->  TCP  -->  80  --> IP
SSH   -->  TCP  -->  22  --> IP
MYSQL -->  TCP  --> 3306 --> IP
* Outbound:
All traffic.

