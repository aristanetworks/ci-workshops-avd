# SITE2_FABRIC

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
| SITE2_FABRIC | l3leaf | s2-brdr1 | 192.168.0.200/24 | cEOS | Provisioned | - |
| SITE2_FABRIC | l3leaf | s2-brdr2 | 192.168.0.201/24 | cEOS | Provisioned | - |
| SITE2_FABRIC | l3leaf | s2-leaf1 | 192.168.0.22/24 | cEOS | Provisioned | - |
| SITE2_FABRIC | l3leaf | s2-leaf2 | 192.168.0.23/24 | cEOS | Provisioned | - |
| SITE2_FABRIC | l3leaf | s2-leaf3 | 192.168.0.24/24 | cEOS | Provisioned | - |
| SITE2_FABRIC | l3leaf | s2-leaf4 | 192.168.0.25/24 | cEOS | Provisioned | - |
| SITE2_FABRIC | spine | s2-spine1 | 192.168.0.20/24 | cEOS | Provisioned | - |
| SITE2_FABRIC | spine | s2-spine2 | 192.168.0.21/24 | cEOS | Provisioned | - |

> Provision status is based on Ansible inventory declaration and do not represent real status from CloudVision.

### Fabric Switches with inband Management IP

| POD | Type | Node | Management IP | Inband Interface |
| --- | ---- | ---- | ------------- | ---------------- |

## Fabric Topology

| Type | Node | Node Interface | Peer Type | Peer Node | Peer Interface |
| ---- | ---- | -------------- | --------- | ----------| -------------- |
| l3leaf | s2-brdr1 | Ethernet1 | mlag_peer | s2-brdr2 | Ethernet1 |
| l3leaf | s2-brdr1 | Ethernet2 | spine | s2-spine1 | Ethernet7 |
| l3leaf | s2-brdr1 | Ethernet3 | spine | s2-spine2 | Ethernet7 |
| l3leaf | s2-brdr1 | Ethernet6 | mlag_peer | s2-brdr2 | Ethernet6 |
| l3leaf | s2-brdr2 | Ethernet2 | spine | s2-spine1 | Ethernet8 |
| l3leaf | s2-brdr2 | Ethernet3 | spine | s2-spine2 | Ethernet8 |
| l3leaf | s2-leaf1 | Ethernet1 | mlag_peer | s2-leaf2 | Ethernet1 |
| l3leaf | s2-leaf1 | Ethernet2 | spine | s2-spine1 | Ethernet2 |
| l3leaf | s2-leaf1 | Ethernet3 | spine | s2-spine2 | Ethernet2 |
| l3leaf | s2-leaf1 | Ethernet6 | mlag_peer | s2-leaf2 | Ethernet6 |
| l3leaf | s2-leaf2 | Ethernet2 | spine | s2-spine1 | Ethernet3 |
| l3leaf | s2-leaf2 | Ethernet3 | spine | s2-spine2 | Ethernet3 |
| l3leaf | s2-leaf3 | Ethernet1 | mlag_peer | s2-leaf4 | Ethernet1 |
| l3leaf | s2-leaf3 | Ethernet2 | spine | s2-spine1 | Ethernet4 |
| l3leaf | s2-leaf3 | Ethernet3 | spine | s2-spine2 | Ethernet4 |
| l3leaf | s2-leaf3 | Ethernet6 | mlag_peer | s2-leaf4 | Ethernet6 |
| l3leaf | s2-leaf4 | Ethernet2 | spine | s2-spine1 | Ethernet5 |
| l3leaf | s2-leaf4 | Ethernet3 | spine | s2-spine2 | Ethernet5 |

## Fabric IP Allocation

### Fabric Point-To-Point Links

| Uplink IPv4 Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ---------------- | ------------------- | ------------------ | ------------------ |
| 172.16.2.0/24 | 256 | 24 | 9.38 % |

### Point-To-Point Links Node Allocation

| Node | Node Interface | Node IP Address | Peer Node | Peer Interface | Peer IP Address |
| ---- | -------------- | --------------- | --------- | -------------- | --------------- |
| s2-brdr1 | Ethernet2 | 172.16.2.17/31 | s2-spine1 | Ethernet7 | 172.16.2.16/31 |
| s2-brdr1 | Ethernet3 | 172.16.2.19/31 | s2-spine2 | Ethernet7 | 172.16.2.18/31 |
| s2-brdr2 | Ethernet2 | 172.16.2.21/31 | s2-spine1 | Ethernet8 | 172.16.2.20/31 |
| s2-brdr2 | Ethernet3 | 172.16.2.23/31 | s2-spine2 | Ethernet8 | 172.16.2.22/31 |
| s2-leaf1 | Ethernet2 | 172.16.2.1/31 | s2-spine1 | Ethernet2 | 172.16.2.0/31 |
| s2-leaf1 | Ethernet3 | 172.16.2.3/31 | s2-spine2 | Ethernet2 | 172.16.2.2/31 |
| s2-leaf2 | Ethernet2 | 172.16.2.5/31 | s2-spine1 | Ethernet3 | 172.16.2.4/31 |
| s2-leaf2 | Ethernet3 | 172.16.2.7/31 | s2-spine2 | Ethernet3 | 172.16.2.6/31 |
| s2-leaf3 | Ethernet2 | 172.16.2.9/31 | s2-spine1 | Ethernet4 | 172.16.2.8/31 |
| s2-leaf3 | Ethernet3 | 172.16.2.11/31 | s2-spine2 | Ethernet4 | 172.16.2.10/31 |
| s2-leaf4 | Ethernet2 | 172.16.2.13/31 | s2-spine1 | Ethernet5 | 172.16.2.12/31 |
| s2-leaf4 | Ethernet3 | 172.16.2.15/31 | s2-spine2 | Ethernet5 | 172.16.2.14/31 |

### Loopback Interfaces (BGP EVPN Peering)

| Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------- | ------------------- | ------------------ | ------------------ |
| 10.250.2.0/24 | 256 | 8 | 3.13 % |

### Loopback0 Interfaces Node Allocation

| POD | Node | Loopback0 |
| --- | ---- | --------- |
| SITE2_FABRIC | s2-brdr1 | 10.250.2.7/32 |
| SITE2_FABRIC | s2-brdr2 | 10.250.2.8/32 |
| SITE2_FABRIC | s2-leaf1 | 10.250.2.3/32 |
| SITE2_FABRIC | s2-leaf2 | 10.250.2.4/32 |
| SITE2_FABRIC | s2-leaf3 | 10.250.2.5/32 |
| SITE2_FABRIC | s2-leaf4 | 10.250.2.6/32 |
| SITE2_FABRIC | s2-spine1 | 10.250.2.1/32 |
| SITE2_FABRIC | s2-spine2 | 10.250.2.2/32 |

### VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)

| VTEP Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------------ | ------------------- | ------------------ | ------------------ |
| 10.255.2.0/24 | 256 | 6 | 2.35 % |

### VTEP Loopback Node allocation

| POD | Node | Loopback1 |
| --- | ---- | --------- |
| SITE2_FABRIC | s2-brdr1 | 10.255.2.7/32 |
| SITE2_FABRIC | s2-brdr2 | 10.255.2.7/32 |
| SITE2_FABRIC | s2-leaf1 | 10.255.2.3/32 |
| SITE2_FABRIC | s2-leaf2 | 10.255.2.3/32 |
| SITE2_FABRIC | s2-leaf3 | 10.255.2.5/32 |
| SITE2_FABRIC | s2-leaf4 | 10.255.2.5/32 |
