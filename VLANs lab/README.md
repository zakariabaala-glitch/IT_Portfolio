# VLANs, Trunking, and Router-on-a-Stick Lab

This Packet Tracer lab demonstrates VLAN configuration, trunking between switches, and inter-VLAN routing using **router-on-a-stick**.

---

## 📝 Lab Objectives
1. Configure switch interfaces connected to PCs as **access ports** in the correct VLAN.
2. Configure the link between **SW1** and **SW2** as a **trunk**:
   - Allow only the necessary VLANs.
   - Use an **unused VLAN as the native VLAN**.
   - Ensure all necessary VLANs exist on both switches.
3. Configure the connection between **SW2** and **R1** using **router-on-a-stick**:
   - Create subinterfaces on R1.
   - Assign the **last usable IP address** of each subnet to the corresponding subinterface.
4. Verify configuration by testing connectivity:
   - All PCs should be able to **ping each other** across VLANs.

---

## ⚙️ Key Configurations

### Switches
- **Access Ports**: Assigned to correct VLANs for connected PCs.
- **Trunk Port**: Between SW1 and SW2.
  - Only required VLANs allowed.
  - Native VLAN set to an unused VLAN.

### Router (R1)
- Configured with **subinterfaces** (router-on-a-stick).
- Each subinterface uses the **last usable IP** from its subnet.
- Provides **inter-VLAN routing**.

---

## ✅ Verification
- Use `ping` from any PC to test connectivity across VLANs.
- Confirm VLAN membership with:
  ```bash
  show vlan brief
  show interfaces trunk

