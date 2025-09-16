🖧 VLSM & Static Routing Lab
🎯 Objective

Subnet the 192.168.5.0/24 network using VLSM to provide addressing for:

LAN1 (PC1 and R1)

LAN2 (PC2 and R1)

LAN3 (PC3 and R2)

Point-to-point link between R1 and R2

Assign:

First usable IP → PC in each LAN

Last usable IP → Router interface in each LAN

Configure static routes so that all PCs can communicate across the routers.

📝 Tasks Completed

Designed and applied a VLSM subnetting plan

Assigned IP addresses according to requirements

Configured router interfaces and LAN hosts

Implemented static routing on both routers

Verified full end-to-end connectivity

✅ Verification

PCs were assigned the first usable IP in each subnet

Router interfaces were assigned the last usable IP in each subnet

Successful connectivity tests:
  ping between PC1 and PC2
  ping between PC1 and PC3
  ping between PC1 ↔ R2 and PC3 ↔ R1
