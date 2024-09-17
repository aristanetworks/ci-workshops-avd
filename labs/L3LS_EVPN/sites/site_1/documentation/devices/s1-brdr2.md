# s1-brdr2

## Table of Contents

- [Management](#management)
  - [Management Interfaces](#management-interfaces)
  - [DNS Domain](#dns-domain)
  - [NTP](#ntp)
  - [Management API HTTP](#management-api-http)
- [Authentication](#authentication)
  - [Local Users](#local-users)
  - [AAA Authorization](#aaa-authorization)
- [Monitoring](#monitoring)
  - [TerminAttr Daemon](#terminattr-daemon)
  - [Logging](#logging)
- [MLAG](#mlag)
  - [MLAG Summary](#mlag-summary)
  - [MLAG Device Configuration](#mlag-device-configuration)
- [Spanning Tree](#spanning-tree)
  - [Spanning Tree Summary](#spanning-tree-summary)
  - [Spanning Tree Device Configuration](#spanning-tree-device-configuration)
- [Internal VLAN Allocation Policy](#internal-vlan-allocation-policy)
  - [Internal VLAN Allocation Policy Summary](#internal-vlan-allocation-policy-summary)
  - [Internal VLAN Allocation Policy Device Configuration](#internal-vlan-allocation-policy-device-configuration)
- [VLANs](#vlans)
  - [VLANs Summary](#vlans-summary)
  - [VLANs Device Configuration](#vlans-device-configuration)
- [Interfaces](#interfaces)
  - [Ethernet Interfaces](#ethernet-interfaces)
  - [Port-Channel Interfaces](#port-channel-interfaces)
  - [Loopback Interfaces](#loopback-interfaces)
  - [VLAN Interfaces](#vlan-interfaces)
  - [VXLAN Interface](#vxlan-interface)
- [Routing](#routing)
  - [Service Routing Protocols Model](#service-routing-protocols-model)
  - [Virtual Router MAC Address](#virtual-router-mac-address)
  - [IP Routing](#ip-routing)
  - [IPv6 Routing](#ipv6-routing)
  - [Static Routes](#static-routes)
  - [Router BGP](#router-bgp)
- [BFD](#bfd)
  - [Router BFD](#router-bfd)
- [Multicast](#multicast)
  - [IP IGMP Snooping](#ip-igmp-snooping)
- [Filters](#filters)
  - [Prefix-lists](#prefix-lists)
  - [Route-maps](#route-maps)
- [VRF Instances](#vrf-instances)
  - [VRF Instances Summary](#vrf-instances-summary)
  - [VRF Instances Device Configuration](#vrf-instances-device-configuration)

## Management

### Management Interfaces

#### Management Interfaces Summary

##### IPv4

| Management Interface | Description | Type | VRF | IP Address | Gateway |
| -------------------- | ----------- | ---- | --- | ---------- | ------- |
| Management0 | oob_management | oob | default | 192.168.0.101/24 | 192.168.0.1 |

##### IPv6

| Management Interface | Description | Type | VRF | IPv6 Address | IPv6 Gateway |
| -------------------- | ----------- | ---- | --- | ------------ | ------------ |
| Management0 | oob_management | oob | default | - | - |

#### Management Interfaces Device Configuration

```eos
!
interface Management0
   description oob_management
   no shutdown
   ip address 192.168.0.101/24
```

### DNS Domain

DNS domain: atd.lab

#### DNS Domain Device Configuration

```eos
dns domain atd.lab
!
```

### NTP

#### NTP Summary

##### NTP Servers

| Server | VRF | Preferred | Burst | iBurst | Version | Min Poll | Max Poll | Local-interface | Key |
| ------ | --- | --------- | ----- | ------ | ------- | -------- | -------- | --------------- | --- |
| 192.168.0.1 | - | - | - | True | - | - | - | Management0 | - |

#### NTP Device Configuration

```eos
!
ntp server 192.168.0.1 iburst local-interface Management0
```

### Management API HTTP

#### Management API HTTP Summary

| HTTP | HTTPS | Default Services |
| ---- | ----- | ---------------- |
| False | True | - |

#### Management API VRF Access

| VRF Name | IPv4 ACL | IPv6 ACL |
| -------- | -------- | -------- |
| default | - | - |

#### Management API HTTP Device Configuration

```eos
!
management api http-commands
   protocol https
   no shutdown
   !
   vrf default
      no shutdown
```

## Authentication

### Local Users

#### Local Users Summary

| User | Privilege | Role | Disabled | Shell |
| ---- | --------- | ---- | -------- | ----- |
| arista | 15 | network-admin | False | - |

#### Local Users Device Configuration

```eos
!
username arista privilege 15 role network-admin secret sha512 <removed>
username arista ssh-key ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC+KtN0VMvBH0eWXuy+IuCWDRIsC1x1k7P8KMIRQ9mIajYjMdx4YODqEVJiXoc6i9970cTX+5SQJxAQZP8G7ahw4fkCRQis/xfVW8kg7EBVJXOOfGOiyo53mkAbc10qAcEzOsE0bSJNHPHTnNaIOtk9wGM46N22yOuHNHgOIa0N3L4SypBLK0kaOQbt+y85mq0KYRYm8hWzIEPhLK70AIaQzvbM92zMrvahGka2eF/qUDFyuFfiIYGs/3cdt9KuO9+IwpwuokUbNU4Ply59ipiicJCssldpvBoy+7W07iUTC0cwoI5ZGu0bTzojfGZUvhCsrqBVxEtLMo3dM+jYvCG7 arista@ase-nbatman-1-a55c9949-eos.c.atds-280712.internal
```

### AAA Authorization

#### AAA Authorization Summary

| Type | User Stores |
| ---- | ----------- |
| Exec | local |

Authorization for configuration commands is disabled.

#### AAA Authorization Device Configuration

```eos
aaa authorization exec default local
!
```

## Monitoring

### TerminAttr Daemon

#### TerminAttr Daemon Summary

| CV Compression | CloudVision Servers | VRF | Authentication | Smash Excludes | Ingest Exclude | Bypass AAA |
| -------------- | ------------------- | --- | -------------- | -------------- | -------------- | ---------- |
| gzip | 192.168.0.5:9910 | - | token,/tmp/token | ale,flexCounter,hardware,kni,pulse,strata | /Sysdb/cell/1/agent,/Sysdb/cell/2/agent | False |

#### TerminAttr Daemon Device Configuration

```eos
!
daemon TerminAttr
   exec /usr/bin/TerminAttr -cvaddr=192.168.0.5:9910 -cvauth=token,/tmp/token -smashexcludes=ale,flexCounter,hardware,kni,pulse,strata -ingestexclude=/Sysdb/cell/1/agent,/Sysdb/cell/2/agent -taillogs
   no shutdown
```

### Logging

#### Logging Servers and Features Summary

| Type | Level |
| -----| ----- |

| VRF | Source Interface |
| --- | ---------------- |
| default | Management0 |

| VRF | Hosts | Ports | Protocol |
| --- | ----- | ----- | -------- |
| default | 10.200.0.108 | Default | UDP |
| default | 10.200.1.108 | Default | UDP |

#### Logging Servers and Features Device Configuration

```eos
!
logging host 10.200.0.108
logging host 10.200.1.108
logging source-interface Management0
```

## MLAG

### MLAG Summary

| Domain-id | Local-interface | Peer-address | Peer-link |
| --------- | --------------- | ------------ | --------- |
| S1_BRDR | Vlan4094 | 10.251.1.8 | Port-Channel1 |

Dual primary detection is disabled.

### MLAG Device Configuration

```eos
!
mlag configuration
   domain-id S1_BRDR
   local-interface Vlan4094
   peer-address 10.251.1.8
   peer-link Port-Channel1
   reload-delay mlag 300
   reload-delay non-mlag 330
```

## Spanning Tree

### Spanning Tree Summary

STP mode: **mstp**

#### MSTP Instance and Priority

| Instance(s) | Priority |
| -------- | -------- |
| 0 | 4096 |

#### Global Spanning-Tree Settings

- Spanning Tree disabled for VLANs: **4093-4094**

### Spanning Tree Device Configuration

```eos
!
spanning-tree mode mstp
no spanning-tree vlan-id 4093-4094
spanning-tree mst 0 priority 4096
```

## Internal VLAN Allocation Policy

### Internal VLAN Allocation Policy Summary

| Policy Allocation | Range Beginning | Range Ending |
| ------------------| --------------- | ------------ |
| ascending | 1006 | 1199 |

### Internal VLAN Allocation Policy Device Configuration

```eos
!
vlan internal order ascending range 1006 1199
```

## VLANs

### VLANs Summary

| VLAN ID | Name | Trunk Groups |
| ------- | ---- | ------------ |
| 10 | Ten | - |
| 20 | Twenty | - |
| 3009 | MLAG_iBGP_OVERLAY | LEAF_PEER_L3 |
| 4093 | LEAF_PEER_L3 | LEAF_PEER_L3 |
| 4094 | MLAG_PEER | MLAG |

### VLANs Device Configuration

```eos
!
vlan 10
   name Ten
!
vlan 20
   name Twenty
!
vlan 3009
   name MLAG_iBGP_OVERLAY
   trunk group LEAF_PEER_L3
!
vlan 4093
   name LEAF_PEER_L3
   trunk group LEAF_PEER_L3
!
vlan 4094
   name MLAG_PEER
   trunk group MLAG
```

## Interfaces

### Ethernet Interfaces

#### Ethernet Interfaces Summary

##### L2

| Interface | Description | Mode | VLANs | Native VLAN | Trunk Group | Channel-Group |
| --------- | ----------- | ---- | ----- | ----------- | ----------- | ------------- |
| Ethernet1 | MLAG_PEER_s1-brdr1_Ethernet1 | *trunk | *- | *- | *['LEAF_PEER_L3', 'MLAG'] | 1 |
| Ethernet6 | MLAG_PEER_s1-brdr1_Ethernet6 | *trunk | *- | *- | *['LEAF_PEER_L3', 'MLAG'] | 1 |

*Inherited from Port-Channel Interface

##### IPv4

| Interface | Description | Type | Channel Group | IP Address | VRF |  MTU | Shutdown | ACL In | ACL Out |
| --------- | ----------- | -----| ------------- | ---------- | ----| ---- | -------- | ------ | ------- |
| Ethernet2 | P2P_LINK_TO_S1-SPINE1_Ethernet8 | routed | - | 172.16.1.21/31 | default | 1500 | False | - | - |
| Ethernet3 | P2P_LINK_TO_S1-SPINE2_Ethernet8 | routed | - | 172.16.1.23/31 | default | 1500 | False | - | - |
| Ethernet5 | P2P_LINK_TO_s2-brdr2_Ethernet5 | routed | - | 172.16.255.2/31 | default | 1500 | False | - | - |

#### Ethernet Interfaces Device Configuration

```eos
!
interface Ethernet1
   description MLAG_PEER_s1-brdr1_Ethernet1
   no shutdown
   channel-group 1 mode active
!
interface Ethernet2
   description P2P_LINK_TO_S1-SPINE1_Ethernet8
   no shutdown
   mtu 1500
   no switchport
   ip address 172.16.1.21/31
!
interface Ethernet3
   description P2P_LINK_TO_S1-SPINE2_Ethernet8
   no shutdown
   mtu 1500
   no switchport
   ip address 172.16.1.23/31
!
interface Ethernet5
   description P2P_LINK_TO_s2-brdr2_Ethernet5
   no shutdown
   mtu 1500
   no switchport
   ip address 172.16.255.2/31
!
interface Ethernet6
   description MLAG_PEER_s1-brdr1_Ethernet6
   no shutdown
   channel-group 1 mode active
```

### Port-Channel Interfaces

#### Port-Channel Interfaces Summary

##### L2

| Interface | Description | Type | Mode | VLANs | Native VLAN | Trunk Group | LACP Fallback Timeout | LACP Fallback Mode | MLAG ID | EVPN ESI |
| --------- | ----------- | ---- | ---- | ----- | ----------- | ------------| --------------------- | ------------------ | ------- | -------- |
| Port-Channel1 | MLAG_PEER_s1-brdr1_Po1 | switched | trunk | - | - | ['LEAF_PEER_L3', 'MLAG'] | - | - | - | - |

#### Port-Channel Interfaces Device Configuration

```eos
!
interface Port-Channel1
   description MLAG_PEER_s1-brdr1_Po1
   no shutdown
   switchport
   switchport mode trunk
   switchport trunk group LEAF_PEER_L3
   switchport trunk group MLAG
```

### Loopback Interfaces

#### Loopback Interfaces Summary

##### IPv4

| Interface | Description | VRF | IP Address |
| --------- | ----------- | --- | ---------- |
| Loopback0 | EVPN_Overlay_Peering | default | 10.250.1.8/32 |
| Loopback1 | VTEP_VXLAN_Tunnel_Source | default | 10.255.1.7/32 |

##### IPv6

| Interface | Description | VRF | IPv6 Address |
| --------- | ----------- | --- | ------------ |
| Loopback0 | EVPN_Overlay_Peering | default | - |
| Loopback1 | VTEP_VXLAN_Tunnel_Source | default | - |

#### Loopback Interfaces Device Configuration

```eos
!
interface Loopback0
   description EVPN_Overlay_Peering
   no shutdown
   ip address 10.250.1.8/32
!
interface Loopback1
   description VTEP_VXLAN_Tunnel_Source
   no shutdown
   ip address 10.255.1.7/32
```

### VLAN Interfaces

#### VLAN Interfaces Summary

| Interface | Description | VRF |  MTU | Shutdown |
| --------- | ----------- | --- | ---- | -------- |
| Vlan10 | Ten | OVERLAY | - | False |
| Vlan20 | Twenty | OVERLAY | - | False |
| Vlan3009 | MLAG_PEER_L3_iBGP: vrf OVERLAY | OVERLAY | 1500 | False |
| Vlan4093 | MLAG_PEER_L3_PEERING | default | 1500 | False |
| Vlan4094 | MLAG_PEER | default | 1500 | False |

##### IPv4

| Interface | VRF | IP Address | IP Address Virtual | IP Router Virtual Address | VRRP | ACL In | ACL Out |
| --------- | --- | ---------- | ------------------ | ------------------------- | ---- | ------ | ------- |
| Vlan10 |  OVERLAY  |  -  |  10.10.10.1/24  |  -  |  -  |  -  |  -  |
| Vlan20 |  OVERLAY  |  -  |  10.20.20.1/24  |  -  |  -  |  -  |  -  |
| Vlan3009 |  OVERLAY  |  10.252.1.9/31  |  -  |  -  |  -  |  -  |  -  |
| Vlan4093 |  default  |  10.252.1.9/31  |  -  |  -  |  -  |  -  |  -  |
| Vlan4094 |  default  |  10.251.1.9/31  |  -  |  -  |  -  |  -  |  -  |

#### VLAN Interfaces Device Configuration

```eos
!
interface Vlan10
   description Ten
   no shutdown
   vrf OVERLAY
   ip address virtual 10.10.10.1/24
!
interface Vlan20
   description Twenty
   no shutdown
   vrf OVERLAY
   ip address virtual 10.20.20.1/24
!
interface Vlan3009
   description MLAG_PEER_L3_iBGP: vrf OVERLAY
   no shutdown
   mtu 1500
   vrf OVERLAY
   ip address 10.252.1.9/31
!
interface Vlan4093
   description MLAG_PEER_L3_PEERING
   no shutdown
   mtu 1500
   ip address 10.252.1.9/31
!
interface Vlan4094
   description MLAG_PEER
   no shutdown
   mtu 1500
   no autostate
   ip address 10.251.1.9/31
```

### VXLAN Interface

#### VXLAN Interface Summary

| Setting | Value |
| ------- | ----- |
| Source Interface | Loopback1 |
| UDP port | 4789 |
| EVPN MLAG Shared Router MAC | mlag-system-id |

##### VLAN to VNI, Flood List and Multicast Group Mappings

| VLAN | VNI | Flood List | Multicast Group |
| ---- | --- | ---------- | --------------- |
| 10 | 10010 | - | - |
| 20 | 10020 | - | - |

##### VRF to VNI and Multicast Group Mappings

| VRF | VNI | Multicast Group |
| ---- | --- | --------------- |
| OVERLAY | 10 | - |

#### VXLAN Interface Device Configuration

```eos
!
interface Vxlan1
   description s1-brdr2_VTEP
   vxlan source-interface Loopback1
   vxlan virtual-router encapsulation mac-address mlag-system-id
   vxlan udp-port 4789
   vxlan vlan 10 vni 10010
   vxlan vlan 20 vni 10020
   vxlan vrf OVERLAY vni 10
```

## Routing

### Service Routing Protocols Model

Multi agent routing protocol model enabled

```eos
!
service routing protocols model multi-agent
```

### Virtual Router MAC Address

#### Virtual Router MAC Address Summary

Virtual Router MAC Address: 00:1c:73:00:00:99

#### Virtual Router MAC Address Device Configuration

```eos
!
ip virtual-router mac-address 00:1c:73:00:00:99
```

### IP Routing

#### IP Routing Summary

| VRF | Routing Enabled |
| --- | --------------- |
| default | True |
| OVERLAY | True |

#### IP Routing Device Configuration

```eos
!
ip routing
ip routing vrf OVERLAY
```

### IPv6 Routing

#### IPv6 Routing Summary

| VRF | Routing Enabled |
| --- | --------------- |
| default | False |
| default | false |
| OVERLAY | false |

### Static Routes

#### Static Routes Summary

| VRF | Destination Prefix | Next Hop IP | Exit interface | Administrative Distance | Tag | Route Name | Metric |
| --- | ------------------ | ----------- | -------------- | ----------------------- | --- | ---------- | ------ |
| default | 0.0.0.0/0 | 192.168.0.1 | - | 1 | - | - | - |

#### Static Routes Device Configuration

```eos
!
ip route 0.0.0.0/0 192.168.0.1
```

### Router BGP

ASN Notation: asplain

#### Router BGP Summary

| BGP AS | Router ID |
| ------ | --------- |
| 65103 | 10.250.1.8 |

| BGP Tuning |
| ---------- |
| no bgp default ipv4-unicast |
| maximum-paths 4 ecmp 4 |

#### Router BGP Peer Groups

##### EVPN-OVERLAY-CORE

| Settings | Value |
| -------- | ----- |
| Address Family | evpn |
| Source | Loopback0 |
| BFD | True |
| Ebgp multihop | 15 |
| Send community | all |
| Maximum routes | 0 (no limit) |

##### EVPN-OVERLAY-PEERS

| Settings | Value |
| -------- | ----- |
| Address Family | evpn |
| Source | Loopback0 |
| BFD | True |
| Ebgp multihop | 3 |
| Send community | all |
| Maximum routes | 0 (no limit) |

##### IPv4-UNDERLAY-PEERS

| Settings | Value |
| -------- | ----- |
| Address Family | ipv4 |
| Send community | all |
| Maximum routes | 12000 |

##### MLAG-IPv4-UNDERLAY-PEER

| Settings | Value |
| -------- | ----- |
| Address Family | ipv4 |
| Remote AS | 65103 |
| Next-hop self | True |
| Send community | all |
| Maximum routes | 12000 |

#### BGP Neighbors

| Neighbor | Remote AS | VRF | Shutdown | Send-community | Maximum-routes | Allowas-in | BFD | RIB Pre-Policy Retain | Route-Reflector Client | Passive | TTL Max Hops |
| -------- | --------- | --- | -------- | -------------- | -------------- | ---------- | --- | --------------------- | ---------------------- | ------- | ------------ |
| 10.250.1.1 | 65100 | default | - | Inherited from peer group EVPN-OVERLAY-PEERS | Inherited from peer group EVPN-OVERLAY-PEERS | - | Inherited from peer group EVPN-OVERLAY-PEERS | - | - | - | - |
| 10.250.1.2 | 65100 | default | - | Inherited from peer group EVPN-OVERLAY-PEERS | Inherited from peer group EVPN-OVERLAY-PEERS | - | Inherited from peer group EVPN-OVERLAY-PEERS | - | - | - | - |
| 10.250.2.8 | 65203 | default | - | Inherited from peer group EVPN-OVERLAY-CORE | Inherited from peer group EVPN-OVERLAY-CORE | - | Inherited from peer group EVPN-OVERLAY-CORE | - | - | - | - |
| 10.252.1.8 | Inherited from peer group MLAG-IPv4-UNDERLAY-PEER | default | - | Inherited from peer group MLAG-IPv4-UNDERLAY-PEER | Inherited from peer group MLAG-IPv4-UNDERLAY-PEER | - | - | - | - | - | - |
| 172.16.1.20 | 65100 | default | - | Inherited from peer group IPv4-UNDERLAY-PEERS | Inherited from peer group IPv4-UNDERLAY-PEERS | - | - | - | - | - | - |
| 172.16.1.22 | 65100 | default | - | Inherited from peer group IPv4-UNDERLAY-PEERS | Inherited from peer group IPv4-UNDERLAY-PEERS | - | - | - | - | - | - |
| 172.16.255.3 | 65203 | default | - | Inherited from peer group IPv4-UNDERLAY-PEERS | Inherited from peer group IPv4-UNDERLAY-PEERS | - | - | - | - | - | - |
| 10.252.1.8 | Inherited from peer group MLAG-IPv4-UNDERLAY-PEER | OVERLAY | - | Inherited from peer group MLAG-IPv4-UNDERLAY-PEER | Inherited from peer group MLAG-IPv4-UNDERLAY-PEER | - | - | - | - | - | - |

#### Router BGP EVPN Address Family

##### EVPN Peer Groups

| Peer Group | Activate | Encapsulation |
| ---------- | -------- | ------------- |
| EVPN-OVERLAY-CORE | True | default |
| EVPN-OVERLAY-PEERS | True | default |

##### EVPN DCI Gateway Summary

| Settings | Value |
| -------- | ----- |
| Remote Domain Peer Groups | EVPN-OVERLAY-CORE |
| L3 Gateway Configured | True |
| L3 Gateway Inter-domain | True |

#### Router BGP VLANs

| VLAN | Route-Distinguisher | Both Route-Target | Import Route Target | Export Route-Target | Redistribute |
| ---- | ------------------- | ----------------- | ------------------- | ------------------- | ------------ |
| 10 | 10.250.1.8:10010 | 10010:10010<br>remote 10010:10010 | - | - | learned |
| 20 | 10.250.1.8:10020 | 10020:10020<br>remote 10020:10020 | - | - | learned |

#### Router BGP VRFs

| VRF | Route-Distinguisher | Redistribute |
| --- | ------------------- | ------------ |
| OVERLAY | 10.250.1.8:10 | connected |

#### Router BGP Device Configuration

```eos
!
router bgp 65103
   router-id 10.250.1.8
   maximum-paths 4 ecmp 4
   no bgp default ipv4-unicast
   neighbor EVPN-OVERLAY-CORE peer group
   neighbor EVPN-OVERLAY-CORE update-source Loopback0
   neighbor EVPN-OVERLAY-CORE bfd
   neighbor EVPN-OVERLAY-CORE ebgp-multihop 15
   neighbor EVPN-OVERLAY-CORE send-community
   neighbor EVPN-OVERLAY-CORE maximum-routes 0
   neighbor EVPN-OVERLAY-PEERS peer group
   neighbor EVPN-OVERLAY-PEERS update-source Loopback0
   neighbor EVPN-OVERLAY-PEERS bfd
   neighbor EVPN-OVERLAY-PEERS ebgp-multihop 3
   neighbor EVPN-OVERLAY-PEERS password 7 <removed>
   neighbor EVPN-OVERLAY-PEERS send-community
   neighbor EVPN-OVERLAY-PEERS maximum-routes 0
   neighbor IPv4-UNDERLAY-PEERS peer group
   neighbor IPv4-UNDERLAY-PEERS password 7 <removed>
   neighbor IPv4-UNDERLAY-PEERS send-community
   neighbor IPv4-UNDERLAY-PEERS maximum-routes 12000
   neighbor MLAG-IPv4-UNDERLAY-PEER peer group
   neighbor MLAG-IPv4-UNDERLAY-PEER remote-as 65103
   neighbor MLAG-IPv4-UNDERLAY-PEER next-hop-self
   neighbor MLAG-IPv4-UNDERLAY-PEER description s1-brdr1
   neighbor MLAG-IPv4-UNDERLAY-PEER password 7 <removed>
   neighbor MLAG-IPv4-UNDERLAY-PEER send-community
   neighbor MLAG-IPv4-UNDERLAY-PEER maximum-routes 12000
   neighbor MLAG-IPv4-UNDERLAY-PEER route-map RM-MLAG-PEER-IN in
   neighbor 10.250.1.1 peer group EVPN-OVERLAY-PEERS
   neighbor 10.250.1.1 remote-as 65100
   neighbor 10.250.1.1 description s1-spine1
   neighbor 10.250.1.2 peer group EVPN-OVERLAY-PEERS
   neighbor 10.250.1.2 remote-as 65100
   neighbor 10.250.1.2 description s1-spine2
   neighbor 10.250.2.8 peer group EVPN-OVERLAY-CORE
   neighbor 10.250.2.8 remote-as 65203
   neighbor 10.250.2.8 description s2-brdr2
   neighbor 10.252.1.8 peer group MLAG-IPv4-UNDERLAY-PEER
   neighbor 10.252.1.8 description s1-brdr1
   neighbor 172.16.1.20 peer group IPv4-UNDERLAY-PEERS
   neighbor 172.16.1.20 remote-as 65100
   neighbor 172.16.1.20 description s1-spine1_Ethernet8
   neighbor 172.16.1.22 peer group IPv4-UNDERLAY-PEERS
   neighbor 172.16.1.22 remote-as 65100
   neighbor 172.16.1.22 description s1-spine2_Ethernet8
   neighbor 172.16.255.3 peer group IPv4-UNDERLAY-PEERS
   neighbor 172.16.255.3 remote-as 65203
   neighbor 172.16.255.3 description s2-brdr2
   redistribute connected route-map RM-CONN-2-BGP
   !
   vlan 10
      rd 10.250.1.8:10010
      rd evpn domain remote 10.250.1.8:10010
      route-target both 10010:10010
      route-target import export evpn domain remote 10010:10010
      redistribute learned
   !
   vlan 20
      rd 10.250.1.8:10020
      rd evpn domain remote 10.250.1.8:10020
      route-target both 10020:10020
      route-target import export evpn domain remote 10020:10020
      redistribute learned
   !
   address-family evpn
      neighbor EVPN-OVERLAY-CORE activate
      neighbor EVPN-OVERLAY-CORE domain remote
      neighbor EVPN-OVERLAY-PEERS activate
      neighbor default next-hop-self received-evpn-routes route-type ip-prefix inter-domain
   !
   address-family ipv4
      no neighbor EVPN-OVERLAY-CORE activate
      no neighbor EVPN-OVERLAY-PEERS activate
      neighbor IPv4-UNDERLAY-PEERS activate
      neighbor MLAG-IPv4-UNDERLAY-PEER activate
   !
   vrf OVERLAY
      rd 10.250.1.8:10
      route-target import evpn 10:10
      route-target export evpn 10:10
      router-id 10.250.1.8
      neighbor 10.252.1.8 peer group MLAG-IPv4-UNDERLAY-PEER
      redistribute connected
```

## BFD

### Router BFD

#### Router BFD Multihop Summary

| Interval | Minimum RX | Multiplier |
| -------- | ---------- | ---------- |
| 300 | 300 | 3 |

#### Router BFD Device Configuration

```eos
!
router bfd
   multihop interval 300 min-rx 300 multiplier 3
```

## Multicast

### IP IGMP Snooping

#### IP IGMP Snooping Summary

| IGMP Snooping | Fast Leave | Interface Restart Query | Proxy | Restart Query Interval | Robustness Variable |
| ------------- | ---------- | ----------------------- | ----- | ---------------------- | ------------------- |
| Enabled | - | - | - | - | - |

#### IP IGMP Snooping Device Configuration

```eos
```

## Filters

### Prefix-lists

#### Prefix-lists Summary

##### PL-LOOPBACKS-EVPN-OVERLAY

| Sequence | Action |
| -------- | ------ |
| 10 | permit 10.250.1.0/24 eq 32 |
| 20 | permit 10.255.1.0/24 eq 32 |

#### Prefix-lists Device Configuration

```eos
!
ip prefix-list PL-LOOPBACKS-EVPN-OVERLAY
   seq 10 permit 10.250.1.0/24 eq 32
   seq 20 permit 10.255.1.0/24 eq 32
```

### Route-maps

#### Route-maps Summary

##### RM-CONN-2-BGP

| Sequence | Type | Match | Set | Sub-Route-Map | Continue |
| -------- | ---- | ----- | --- | ------------- | -------- |
| 10 | permit | ip address prefix-list PL-LOOPBACKS-EVPN-OVERLAY | - | - | - |

##### RM-MLAG-PEER-IN

| Sequence | Type | Match | Set | Sub-Route-Map | Continue |
| -------- | ---- | ----- | --- | ------------- | -------- |
| 10 | permit | - | origin incomplete | - | - |

#### Route-maps Device Configuration

```eos
!
route-map RM-CONN-2-BGP permit 10
   match ip address prefix-list PL-LOOPBACKS-EVPN-OVERLAY
!
route-map RM-MLAG-PEER-IN permit 10
   description Make routes learned over MLAG Peer-link less preferred on spines to ensure optimal routing
   set origin incomplete
```

## VRF Instances

### VRF Instances Summary

| VRF Name | IP Routing |
| -------- | ---------- |
| OVERLAY | enabled |

### VRF Instances Device Configuration

```eos
!
vrf instance OVERLAY
```
