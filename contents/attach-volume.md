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
## Steps

- Restart instances after mount volume.
```sh
$ sudo blkid
$ sudo vim /etc/fstab
UUID=<UUIDcode> /<pathmount> <type> defaults,nofail 0 2
```

## Final

```sh
$ sudo umount /<pathmount>
$ sudo mount -a
```

## Restart and check

- Restart system.
```sh
$ lsblk
```