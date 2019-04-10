# HOSTNAME

## To change the system hostname to a public DNS name
```
$ sudo hostnamectl set-hostname webserver.mydomain.com
```
## To change the system hostname without a public DNS name
* For Amazon Linux 2: Use the hostnamectl command to set your hostname to reflect the desired system hostname: (such as webserver)
```
$ sudo hostnamectl set-hostname webserver.localdomain
```
* Open the /etc/hosts file in your favorite text editor and change the entry beginning with 127.0.0.1 to match the example below, substituting your own hostname. 
```
127.0.0.1 webserver.localdomain webserver localhost4 localhost4.localdomain4
```

## Reboot the instance to pick up the new hostname
* Your prompt shold show the new hostname (up to the first "."), and the hostname command should show the fully-qualified domain name.
```
$ hostname
webserver.localdomain
```