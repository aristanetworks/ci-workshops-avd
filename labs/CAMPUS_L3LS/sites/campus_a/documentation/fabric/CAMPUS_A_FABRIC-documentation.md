# CAMPUS_A_FABRIC

## Table of Contents

- [Fabric Switches and Management IP](#fabric-switches-and-management-ip)
  - [Fabric Switches with inband Management IP](#fabric-switches-with-inband-management-ip)
- [Fabric Topology](#fabric-topology)
- [Fabric IP Allocation](#fabric-ip-allocation)
  - [Fabric Point-To-Point Links](#fabric-point-to-point-links)
  - [Point-To-Point Links Node Allocation](#point-to-point-links-node-allocation)
  - [Loopback Interfaces (BGP EVPN Peering)](#loopback-interfaces-bgp-evpn-peering)
  - [Loopback0 Interfaces Node Allocation](#loopback0-interfaces-node-allocation)
  - [VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)](#vtep-loopback-vxlan-tunnel-source-interfaces-vteps-only)
  - [VTEP Loopback Node allocation](#vtep-loopback-node-allocation)

## Fabric Switches and Management IP

| POD | Type | Node | Management IP | Platform | Provisioned in CloudVision | Serial Number |
| --- | ---- | ---- | ------------- | -------- | -------------------------- | ------------- |
| CAMPUS_A_FABRIC | l3leaf | leaf-1a | 192.168.0.14/24 | cEOS | Provisioned | - |
| CAMPUS_A_FABRIC | l3leaf | leaf-1b | 192.168.0.15/24 | cEOS | Provisioned | - |
| CAMPUS_A_FABRIC | l3leaf | leaf-2a | 192.168.0.16/24 | cEOS | Provisioned | - |
| CAMPUS_A_FABRIC | l3leaf | leaf-3a | 192.168.0.17/24 | cEOS | Provisioned | - |
| CAMPUS_A_FABRIC | l3leaf | leaf-3b | 192.168.0.18/24 | cEOS | Provisioned | - |
| CAMPUS_A_FABRIC | l2leaf | member-leaf-3c | 192.168.0.19/24 | cEOS | Provisioned | - |
| CAMPUS_A_FABRIC | l2leaf | member-leaf-3d | 192.168.0.20/24 | cEOS | Provisioned | - |
| CAMPUS_A_FABRIC | l2leaf | member-leaf-3e | 192.168.0.21/24 | cEOS | Provisioned | - |
| CAMPUS_A_FABRIC | spine | spine-1 | 192.168.0.12/24 | cEOS | Provisioned | - |
| CAMPUS_A_FABRIC | spine | spine-2 | 192.168.0.13/24 | cEOS | Provisioned | - |

> Provision status is based on Ansible inventory declaration and do not represent real status from CloudVision.

### Fabric Switches with inband Management IP

| POD | Type | Node | Management IP | Inband Interface |
| --- | ---- | ---- | ------------- | ---------------- |

## Fabric Topology

| Type | Node | Node Interface | Peer Type | Peer Node | Peer Interface |
| ---- | ---- | -------------- | --------- | --------- | -------------- |
| l3leaf | leaf-1a | Ethernet47 | mlag_peer | leaf-1b | Ethernet47 |
| l3leaf | leaf-1a | Ethernet48 | mlag_peer | leaf-1b | Ethernet48 |
| l3leaf | leaf-1a | Ethernet49 | spine | spine-1 | Ethernet3 |
| l3leaf | leaf-1b | Ethernet49 | spine | spine-2 | Ethernet3 |
| l3leaf | leaf-2a | Ethernet1/1 | spine | spine-1 | Ethernet4 |
| l3leaf | leaf-2a | Ethernet2/1 | spine | spine-2 | Ethernet4 |
| l3leaf | leaf-3a | Ethernet47 | mlag_peer | leaf-3b | Ethernet47 |
| l3leaf | leaf-3a | Ethernet48 | mlag_peer | leaf-3b | Ethernet48 |
| l3leaf | leaf-3a | Ethernet49 | spine | spine-1 | Ethernet5 |
| l3leaf | leaf-3a | Ethernet50 | spine | spine-2 | Ethernet5 |
| l3leaf | leaf-3a | Ethernet51 | l2leaf | member-leaf-3c | Ethernet49 |
| l3leaf | leaf-3a | Ethernet52 | l2leaf | member-leaf-3d | Ethernet49 |
| l3leaf | leaf-3a | Ethernet53/1 | l2leaf | member-leaf-3e | Ethernet49 |
| l3leaf | leaf-3b | Ethernet49 | spine | spine-1 | Ethernet6 |
| l3leaf | leaf-3b | Ethernet50 | spine | spine-2 | Ethernet6 |
| l3leaf | leaf-3b | Ethernet51 | l2leaf | member-leaf-3c | Ethernet50 |
| l3leaf | leaf-3b | Ethernet52 | l2leaf | member-leaf-3d | Ethernet50 |
| l3leaf | leaf-3b | Ethernet53/1 | l2leaf | member-leaf-3e | Ethernet50 |

## Fabric IP Allocation

### Fabric Point-To-Point Links

| Uplink IPv4 Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ---------------- | ------------------- | ------------------ | ------------------ |
| 172.16.1.0/24 | 256 | 16 | 6.25 % |

### Point-To-Point Links Node Allocation

| Node | Node Interface | Node IP Address | Peer Node | Peer Interface | Peer IP Address |
| ---- | -------------- | --------------- | --------- | -------------- | --------------- |
| leaf-1a | Ethernet49 | 172.16.1.1/31 | spine-1 | Ethernet3 | 172.16.1.0/31 |
| leaf-1b | Ethernet49 | 172.16.1.3/31 | spine-2 | Ethernet3 | 172.16.1.2/31 |
| leaf-2a | Ethernet1/1 | 172.16.1.9/31 | spine-1 | Ethernet4 | 172.16.1.8/31 |
| leaf-2a | Ethernet2/1 | 172.16.1.11/31 | spine-2 | Ethernet4 | 172.16.1.10/31 |
| leaf-3a | Ethernet49 | 172.16.1.13/31 | spine-1 | Ethernet5 | 172.16.1.12/31 |
| leaf-3a | Ethernet50 | 172.16.1.15/31 | spine-2 | Ethernet5 | 172.16.1.14/31 |
| leaf-3b | Ethernet49 | 172.16.1.17/31 | spine-1 | Ethernet6 | 172.16.1.16/31 |
| leaf-3b | Ethernet50 | 172.16.1.19/31 | spine-2 | Ethernet6 | 172.16.1.18/31 |

### Loopback Interfaces (BGP EVPN Peering)

| Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------- | ------------------- | ------------------ | ------------------ |
| 10.1.252.0/24 | 256 | 2 | 0.79 % |
| 10.250.1.0/24 | 256 | 5 | 1.96 % |

### Loopback0 Interfaces Node Allocation

| POD | Node | Loopback0 |
| --- | ---- | --------- |
| CAMPUS_A_FABRIC | leaf-1a | 10.250.1.3/32 |
| CAMPUS_A_FABRIC | leaf-1b | 10.250.1.4/32 |
| CAMPUS_A_FABRIC | leaf-2a | 10.250.1.5/32 |
| CAMPUS_A_FABRIC | leaf-3a | 10.250.1.6/32 |
| CAMPUS_A_FABRIC | leaf-3b | 10.250.1.7/32 |
| CAMPUS_A_FABRIC | spine-1 | 10.1.252.1/32 |
| CAMPUS_A_FABRIC | spine-2 | 10.1.252.2/32 |

### VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)

| VTEP Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------------ | ------------------- | ------------------ | ------------------ |
| 10.255.255.0/24 | 256 | 5 | 1.96 % |

### VTEP Loopback Node allocation

| POD | Node | Loopback1 |
| --- | ---- | --------- |
| CAMPUS_A_FABRIC | leaf-1a | 10.255.255.3/32 |
| CAMPUS_A_FABRIC | leaf-1b | 10.255.255.3/32 |
| CAMPUS_A_FABRIC | leaf-2a | 10.255.255.5/32 |
| CAMPUS_A_FABRIC | leaf-3a | 10.255.255.6/32 |
| CAMPUS_A_FABRIC | leaf-3b | 10.255.255.6/32 |
