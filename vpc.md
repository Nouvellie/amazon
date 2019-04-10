# VPC

## Steps
* Create a vpc:
```
1. Name tag: vpc-main, vpc-1, etc.
2. IPv4 CIDR block: 172.31.0.0/16.
3. IPv6 CIDR block: No block.
4. Tenancy: Default. (dedicate is better, high cost)
```
* Subnet:
```
1. Name tag: name-172.31.0.0-east-1a. (1a, 1b, 1c, 1d, 1e, 1f)
2. VPC: select name tag of vpc-main.
3. Availability zone: same of name tag. (1a, 1b, 1c, 1d, 1e, 1f)
4. IPv4 CIDR block: 172.31.0.0/20. (172.31.0.0/20, 172.31.16.0/20, 172.31.32.0/20, etc)
```
* Internet gateway:
```
1. Name tag: vpc name.
2. Attach to vpc.
```
* Route table:
```
It's created with vpc. We have to associate the route table with the created internet gateway.
```
* Security group:
```
It must be created associated to the main id of the vpc.
```