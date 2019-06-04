# ATTACH VOLUME
## Commands
#### List block devices:

```sh
$ lsblk
```

The new disk will appear associated with <nvme0n1>, <nvme1n1>, etc.

#### Check if the volume has any data using the following command:

```sh
$ sudo file -s /dev/<nvme0n1>
```

#### Format the volume to ext4 filesystem  using the following command:

```sh
$ sudo mkfs -t ext4 /dev/<nvme0n1>
```

#### Create a directory of your choice to mount our new ext4 volume:

```sh
$ sudo mkdir /<custom>/<attach>
```

#### Mount:

```sh
$ sudo mount /dev/<nvme0n1> /<custom>/<attach>
```

# To add permantly ssd to ec2
## Fstab conf

```sh
$ sudo vim /etc/fstab
```

## [fstab]

```sh
/dev/<nvme0n1> /<custom>/<attach> ext4 errors=remount-ro 0 2
```

#### Check if the fstab file has any error:

```sh
$ sudo mount -a
```