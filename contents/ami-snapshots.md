# AMI AND SNAPSHOTS

## AMIs
* Create:
```
Option "create image" over the instance we want, it will be created with the associated volume.
```
* Instance from AMIs:
```
We create an EC2 instance from our AMIs, it comes with the snapshot associated with the AMI. (ssd/hdd and key pair settings are available for changes)
```
## Snapshots
* Create:
```
Option "create snapshot" over the volume we want. 
```
* Associated:
```
The created instance of an AMI already has the snapshot associated with it, yet the volume can be useful if we need it as a secondary volume.
```
## AMI export
```
Any AMI can be exported to a new region in a "copy AMI" option on top of the main AMI itself, including new permissions.
When an instance is created by an AMI backup, the volume is also added, but the termination mode can be set.
```