# Network Requirements
Typical mining process running stratum+tcp protocol will only require several kb/s network bandwidth.

## LAN > 1000 hosts
Due to ARP table limitation, you will need to sub divide your LAN, by using VLAN or sub-router. Typically each sub-router + switches handles 100~1000 hosts.


### Subnet and DHCP pool
You will need to adjust default router and DHCP pool larger from `255.255.255.0` to `255.255.252.0` to accommodate 1024 hosts.

## Common Problems

### IP Address Duplication



# Power Requirements





# Cooling Requirements
