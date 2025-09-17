🖧 Inter-VLAN Routing with Multilayer Switch
🎯 Objective

Replace Router-on-a-Stick (ROAS) between R1 and SW2 with a point-to-point Layer 3 connection.

Configure SVIs (Switch Virtual Interfaces) on SW2 for each VLAN.

Assign the last usable IP address of each subnet to the SVIs.

Configure a default route on SW2 using R1’s G0/0 as the next hop.

Verify inter-VLAN connectivity and Internet reachability.

📝 Tasks Completed

Converted R1–SW2 link from ROAS to a Layer 3 routed connection.

Configured SVIs on SW2.

Assigned IP addresses (last usable in each subnet) to the SVIs.

Configured a default route on SW2 pointing to R1.

✅ Verification

Hosts in VLAN 10, 20, and 30 successfully ping each other via SVIs.

Default route allows SW2 and VLAN hosts to reach the Internet.

ping 1.1.1.1 from any PC succeeds.
