# AMI AND SNAPSHOTS

## AMIs
* Create:
Option "create image" over the instance that we want. It will be created with the volume associated.
* Instance from AMIs:
We create a EC2 instance from our AMIs. It comes with the snapshot associated to the AMI. (ssd/hdd settings and key pair are available for changes)
<br><br>
## Snapshots
* Create:
Option "create snapshot" over the volume that we want. 
* Associated:
The new instance from AMI already have the snapshot associated, but if will be useful if we need a secondary volume.