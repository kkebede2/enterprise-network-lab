# enterprise-network-lab
Enterprise network lab implementing VLANs, inter-VLAN routing, DHCP, OSPF, and ACL-based traffic control using Cisco Packet Tracer.
# Enterprise Network Lab (VLANs, OSPF, DHCP, ACL)

## A brief overview
Designed and implemented a segmented enterprise network using VLANs, inter-VLAN routing (router-on-a-stick), DHCP, OSPF, and ACLs to control traffic between network segments.

---

## Technologies Used
- Cisco Packet Tracer
- VLANs (802.1Q)
- Inter-VLAN Routing
- DHCP
- OSPF
- ACLs

---

## Network Design
- VLAN 10 (HR)
- VLAN 20 (IT)
- Trunk links between switches and routers
- Router-on-a-stick configuration
- Multi-router topology using OSPF

---

## Key Configurations

### VLAN Configuration
- Created VLANs for segmentation
- Assigned access ports to VLANs
- Configured trunk ports between switches and routers

### Routing
- Implemented inter-VLAN routing using subinterfaces
- Configured OSPF for dynamic routing between routers

### DHCP
- Configured DHCP pools for each VLAN
- Automatically assigned IP addresses to hosts

### Security (ACL)
- Implemented ACL to block VLAN 10 → VLAN 20 traffic
- Allowed all other traffic

---

## Testing & Validation

### Successful Connectivity
- PC → Default Gateway (successful)
- Inter-VLAN communication before ACL (successful)

### Blocked Traffic (ACL)
- VLAN 10 → VLAN 20 communication blocked

---

## 📸 Screenshots

### VLAN Configuration
<img width="726" height="715" alt="vlan-config sw1" src="https://github.com/user-attachments/assets/20d2b639-aee4-4cb9-af50-8fe841a4669c" />
<img width="704" height="699" alt="vlan-config sw2" src="https://github.com/user-attachments/assets/5c48e61b-9b9d-4344-b991-b1b8292c1852" />


### Routing Table
<img width="714" height="712" alt="ospf-routing r1" src="https://github.com/user-attachments/assets/8a2aaa0a-6c3a-4d09-9333-1fff17cbec93" />
<img width="696" height="697" alt="ospf-routing r2" src="https://github.com/user-attachments/assets/b0418509-61e9-4e35-b642-f935f4d77211" />


### Successful Ping along with ACL blockage
<img width="709" height="707" alt="successful-ping   ACL" src="https://github.com/user-attachments/assets/53072645-8396-43f2-ad51-a4b9089ddab5" />
