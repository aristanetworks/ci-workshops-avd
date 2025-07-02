# SITE1_FABRIC

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
| SITE1_FABRIC | leaf | s1-leaf1 | 192.168.0.12/24 | cEOS | Provisioned | - |
| SITE1_FABRIC | leaf | s1-leaf2 | 192.168.0.13/24 | cEOS | Provisioned | - |
| SITE1_FABRIC | leaf | s1-leaf3 | 192.168.0.14/24 | cEOS | Provisioned | - |
| SITE1_FABRIC | leaf | s1-leaf4 | 192.168.0.15/24 | cEOS | Provisioned | - |
| SITE1_FABRIC | l3spine | s1-spine1 | 192.168.0.10/24 | cEOS | Provisioned | - |
| SITE1_FABRIC | l3spine | s1-spine2 | 192.168.0.11/24 | cEOS | Provisioned | - |

> Provision status is based on Ansible inventory declaration and do not represent real status from CloudVision.

### Fabric Switches with inband Management IP

| POD | Type | Node | Management IP | Inband Interface |
| --- | ---- | ---- | ------------- | ---------------- |

## Fabric Topology

| Type | Node | Node Interface | Peer Type | Peer Node | Peer Interface |
| ---- | ---- | -------------- | --------- | ----------| -------------- |
| leaf | s1-leaf1 | Ethernet1 | mlag_peer | s1-leaf2 | Ethernet1 |
| leaf | s1-leaf1 | Ethernet2 | l3spine | s1-spine1 | Ethernet2 |
| leaf | s1-leaf1 | Ethernet3 | l3spine | s1-spine2 | Ethernet2 |
| leaf | s1-leaf1 | Ethernet6 | mlag_peer | s1-leaf2 | Ethernet6 |
| leaf | s1-leaf2 | Ethernet2 | l3spine | s1-spine1 | Ethernet3 |
| leaf | s1-leaf2 | Ethernet3 | l3spine | s1-spine2 | Ethernet3 |
| leaf | s1-leaf3 | Ethernet1 | mlag_peer | s1-leaf4 | Ethernet1 |
| leaf | s1-leaf3 | Ethernet2 | l3spine | s1-spine1 | Ethernet4 |
| leaf | s1-leaf3 | Ethernet3 | l3spine | s1-spine2 | Ethernet4 |
| leaf | s1-leaf3 | Ethernet6 | mlag_peer | s1-leaf4 | Ethernet6 |
| leaf | s1-leaf4 | Ethernet2 | l3spine | s1-spine1 | Ethernet5 |
| leaf | s1-leaf4 | Ethernet3 | l3spine | s1-spine2 | Ethernet5 |
| l3spine | s1-spine1 | Ethernet1 | mlag_peer | s1-spine2 | Ethernet1 |
| l3spine | s1-spine1 | Ethernet6 | mlag_peer | s1-spine2 | Ethernet6 |

## Fabric IP Allocation

### Fabric Point-To-Point Links

| Uplink IPv4 Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ---------------- | ------------------- | ------------------ | ------------------ |

### Point-To-Point Links Node Allocation

| Node | Node Interface | Node IP Address | Peer Node | Peer Interface | Peer IP Address |
| ---- | -------------- | --------------- | --------- | -------------- | --------------- |

### Loopback Interfaces (BGP EVPN Peering)

| Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------- | ------------------- | ------------------ | ------------------ |
| 10.1.252.0/24 | 256 | 2 | 0.79 % |

### Loopback0 Interfaces Node Allocation

| POD | Node | Loopback0 |
| --- | ---- | --------- |
| SITE1_FABRIC | s1-spine1 | 10.1.252.1/32 |
| SITE1_FABRIC | s1-spine2 | 10.1.252.2/32 |

### VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)

| VTEP Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------------ | ------------------- | ------------------ | ------------------ |

### VTEP Loopback Node allocation

| POD | Node | Loopback1 |
| --- | ---- | --------- |
