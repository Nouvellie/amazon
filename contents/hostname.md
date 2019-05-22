# HOSTNAME
## To change the system hostname to a public DNS name

```sh
$ sudo hostnamectl set-hostname <webserver.mydomain.com>
```

## To change the system hostname without a public DNS name
#### For Amazon Linux 2: Use the hostnamectl command to set your hostname to reflect the desired system hostname: (such as webserver)

```sh
$ sudo hostnamectl set-hostname --static <myhostname>
```

#### Open the /etc/cloud/cloud.cfg and add the entry.

```sh
$ sudo vim /etc/cloud/cloud.cfg
preserve_hostname: true
```

## Reboot the instance to pick up the new hostname
* Your prompt shold show the new hostname (up to the first "."), and the hostname command should show the fully-qualified domain name.

```sh
$ hostname
<webserver.localdomain>
```