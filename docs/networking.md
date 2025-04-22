# Networking Doc

## Traffic Flow
```
Public Subnet:
Internet <-> Internet Gateway <-> Router <-> Public Route Table <-> Public Subnet <-> Instance

Private Subnet:
Internet <- Internet Gateway <- NAT Gateway <- Router <- Private Route Table <- Private Subnet <- Instance

Private SSH Subnet:
Internet <-> Internet Gateway <-> Bastion Host (in Public Subnet) <-> Router <-> Private Route Table <-> Private Subnet <-> Instance

Public SSH Subnet:
Internet <-> Internet Gateway <-> Router <-> Public Route Table <-> Public Subnet <-> Instance
```