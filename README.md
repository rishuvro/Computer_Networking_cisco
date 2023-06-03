# Computer Networking Cisco

## Index

1. [VLAN](#vlan)
2. [Inter-VLAN Routing](#inter-vlan-routing)
3. [RIP](#rip)
4. [Static Routing](#static-routing)
5. [NAT](#nat)
6. [Server](#server)

## VLAN

VLAN is a custom network that combines one or more local area networks into a logical network. It allows devices from multiple networks to be grouped into one virtual LAN, which is administered like a physical LAN.

To configure VLAN in Cisco Packet Tracer, follow these steps:

1. Assign laptops to VLANs: Configure laptop0 and laptop2 in VLAN 10, and laptop1 and laptop3 in VLAN 20.

2. Set IP addresses for VLANs:
   - VLAN10 IP: 192.168.1.0/24
   - VLAN20 IP: 192.168.2.0/24

3. Configure VLAN on Switch0:
   - Use appropriate commands to configure VLAN on the switch.

4. Configure VLAN on Switch1:
   - Configure VLAN on Switch1 using similar commands.

5. Test VLAN connectivity: Ping between devices in VLAN 10 and VLAN 20 to verify connectivity.

## Inter-VLAN Routing

Inter-VLAN routing is necessary for connecting one VLAN to another. In this case, we connect Router0 to Switch1 for inter-VLAN routing.

To configure inter-VLAN routing:

1. Configure trunking on Switch1:
   - Use appropriate commands to configure trunking on the specified port.

2. Configure inter-VLAN routing on Router0:
   - Access the router CLI and configure inter-VLAN routing.

3. Set the default gateway for each VLAN:
   - Assign default gateways to VLAN10 (192.168.1.1) and VLAN20 (192.168.2.1).

4. Test inter-VLAN routing: Ping between PCs in different VLANs to confirm connectivity.

## RIP

Routing Information Protocol (RIP) is a distance-vector routing protocol. It allows routers to exchange routing tables with their neighbors.

Perform RIP on the following routers:
- Router0
- Router1
- Router3
- Router2

After configuring RIP, test connectivity by pinging interfaces from the laptops.

## NAT

Network Address Translation (NAT) translates private IP addresses into public IP addresses. It helps conserve available IP addresses.

Perform NAT in the topology using a router as the ISP.

Configure static routing in Router3 and Router4.

Graphical user interface, text, application Description automatically generated

Configure NAT and set up the server.

Perform a search to test the network setup.

