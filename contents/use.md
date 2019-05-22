# USE
## Create a security group

This can be used in any case, but if the associated vpc is deleted the security group will be deleted as well.

#### Inbound:


HTTP  -->  TCP  -->  80  --> IP
SSH   -->  TCP  -->  22  --> IP
MYSQL -->  TCP  --> 3306 --> IP

#### Outbound:

All traffic.

## Ssh
#### Information:

A new public ip is generated, which is more easily accessed from ssh. (can be elastic)
IP (IPv4 Public IP) --> <172.31.0.0.>

#### Command:

```sh
$ ssh -i ~<path/file>.pem <user>@<172.31.0.0>
```

#### Chmod the key:

```sh
$ sudo chmod 400 <file>.pem
```

#### Are you sure you want to continue connecting: (ECDSA key fingerprint)

```sh
$ yes
```