# AMI AND SNAPSHOTS

## AMIs
* Create:
```
Option "create image" over the instance that we want. It will be created with the volume associated.
```
* Instance from AMIs:
```
We create an EC2 instance from our AMIs. It comes with the snapshot associated to the AMI. (ssd/hdd settings and key pair are available for changes)
```
## Snapshots
* Create:
```
Option "create snapshot" over the volume that we want. 
```
* Associated:
```
The new instance from AMI already have the snapshot associated, but if will be useful if we need a secondary volume.
```
## AMI export
```
Any AMI can be exported to a new region in an "copy AMI" option over the main AMI itself, including new permissions.
When an instance is created by an AMI backup, the volume is also added, but the delete mode can be configured.
```