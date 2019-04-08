# ELASTIC IP

## Associated address
* First:
```
First of all we create an elastic IP in the EC2 Dashboard, and then we associate the address with the instance that we choose.
```
## VPC settings
* VPC:
```
It is created when the instance is launched.
```
* Internet gateway:
```
Must be created and attached to the VPC that we need.
```
* Network ACL and route table:
```
Associated to the vpc.
```
* Subnet:
```
Associated with the route table and vpc. Must be available in green state.
```