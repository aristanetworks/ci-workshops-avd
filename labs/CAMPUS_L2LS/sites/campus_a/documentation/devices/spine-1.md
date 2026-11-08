# spine-1

## Table of Contents

- [Management](#management)
  - [Management Interfaces](#management-interfaces)
  - [DNS Domain](#dns-domain)
  - [IP Name Servers](#ip-name-servers)
  - [Domain Lookup](#domain-lookup)
  - [NTP](#ntp)
  - [Management API HTTP](#management-api-http)
- [Authentication](#authentication)
  - [Local Users](#local-users)
  - [Enable Password](#enable-password)
  - [AAA Authorization](#aaa-authorization)
- [Monitoring](#monitoring)
  - [TerminAttr Daemon](#terminattr-daemon)
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
- [Routing](#routing)
  - [Service Routing Protocols Model](#service-routing-protocols-model)
  - [Virtual Router MAC Address](#virtual-router-mac-address)
  - [IP Routing](#ip-routing)
  - [IPv6 Routing](#ipv6-routing)
  - [Static Routes](#static-routes)
  - [Router OSPF](#router-ospf)
- [Multicast](#multicast)
  - [IP IGMP Snooping](#ip-igmp-snooping)
- [VRF Instances](#vrf-instances)
  - [VRF Instances Summary](#vrf-instances-summary)
  - [VRF Instances Device Configuration](#vrf-instances-device-configuration)

## Management

### Management Interfaces

#### Management Interfaces Summary

##### IPv4

| Management Interface | Description | Type | VRF | IP Address | Gateway |
| -------------------- | ----------- | ---- | --- | ---------- | ------- |
| Management0 | OOB_MANAGEMENT | oob | default | 192.168.0.12/24 | 192.168.0.1 |

##### IPv6

| Management Interface | Description | Type | VRF | IPv6 Address | IPv6 Gateway | ND RA RX Accept | ND RA Disabled | ND Managed Config Flag |
| -------------------- | ----------- | ---- | --- | ------------ | ------------ | --------------- | -------------- | ---------------------- |
| Management0 | OOB_MANAGEMENT | oob | default | - | - | - | - | - |

#### Management Interfaces Device Configuration

```eos
!
interface Management0
   description OOB_MANAGEMENT
   no shutdown
   ip address 192.168.0.12/24
```

### DNS Domain

DNS domain: atd.lab

#### DNS Domain Device Configuration

```eos
dns domain atd.lab
!
```

### IP Name Servers

#### IP Name Servers Summary

| Name Server | VRF | Priority |
| ----------- | --- | -------- |
| 192.168.0.1 | default | - |

#### IP Name Servers Device Configuration

```eos
ip name-server vrf default 192.168.0.1
```

### Domain Lookup

#### DNS Domain Lookup Summary

| Source interface | vrf |
| ---------------- | --- |
| Management0 | - |

#### DNS Domain Lookup Device Configuration

```eos
ip domain lookup source-interface Management0
```

### NTP

#### NTP Summary

##### NTP Local Interface

| Interface | VRF |
| --------- | --- |
| Management0 | default |

##### NTP Servers

NTP servers VRF: default

| Server | Preferred | Burst | iBurst | Version | Min Poll | Max Poll | Local-interface | Key |
| ------ | --------- | ----- | ------ | ------- | -------- | -------- | --------------- | --- |
| 192.168.0.1 | True | - | True | - | - | - | - | - |

#### NTP Device Configuration

```eos
!
ntp local-interface Management0
ntp server 192.168.0.1 prefer iburst
```

### Management API HTTP

#### Management API HTTP Summary

| HTTP | HTTPS | UNIX-Socket | Default Services | Session Timeout |
| ---- | ----- | ----------- | ---------------- | --------------- |
| False | True | - | - | 1440 minutes |

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
username arista ssh-key ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCrKJ8S5Kv7UmD9vb6aeJ8FaPoKF+TW42RDM4+w4mUDknIGrJ+42QoLskSBm9ngqjQfapckArVW6k/id3qrMaTmnJMVj0ywdFXma6VT1zAVRZOFX3/4bmH1x8pV4dsurXP18u9PBj2HlW/yTyHGPKKkQF2GtmQIoIu1vGwLHlTQC045dGHA5ai4Pd/AIv2L+VF4mWL0EuAx9tCrT5MI14wFNbi1FrtsLMiplw6H3c4eZV/C+AaBuMs26TsAmBuBSQYmOXQ0Y58n8SQMtB07W8v5iOqfJ1VAwQ4q9hVYdABM6YLxTHmNW8mZDBRkXmhrs83GikD6ZGZAseO2qzbTeqon arista@avd-workshop-campus-1-c644c9e8-eos
```

### Enable Password

Enable password has been disabled

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
| gzip | 192.168.0.5:9910 | default | token,/tmp/token | ale,flexCounter,hardware,kni,pulse,strata | - | True |

#### TerminAttr Daemon Device Configuration

```eos
!
daemon TerminAttr
   exec /usr/bin/TerminAttr -cvaddr=192.168.0.5:9910 -cvauth=token,/tmp/token -cvvrf=default -disableaaa -smashexcludes=ale,flexCounter,hardware,kni,pulse,strata -taillogs -cvsourceintf=Management0
   no shutdown
```

## MLAG

### MLAG Summary

| Domain-id | Local-interface | Peer-address | Peer-link |
| --------- | --------------- | ------------ | --------- |
| CAMPUS_A_SPINES | Vlan4094 | 10.1.253.1 | Port-Channel491 |

Dual primary detection is disabled.

### MLAG Device Configuration

```eos
!
mlag configuration
   domain-id CAMPUS_A_SPINES
   local-interface Vlan4094
   peer-address 10.1.253.1
   peer-link Port-Channel491
```

## Spanning Tree

### Spanning Tree Summary

STP mode: **mstp**

#### MSTP Instance and Priority

| Instance(s) | Priority |
| -------- | -------- |
| 0 | 32768 |

#### Global Spanning-Tree Settings

- Spanning Tree disabled for VLANs: **4093-4094**

### Spanning Tree Device Configuration

```eos
!
spanning-tree mode mstp
no spanning-tree vlan-id 4093-4094
spanning-tree mst 0 priority 32768
```

## Internal VLAN Allocation Policy

### Internal VLAN Allocation Policy Summary

| Policy Allocation | Range Beginning | Range Ending |
| ----------------- | --------------- | ------------ |
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
| 110 | IDF1_DATA | - |
| 120 | IDF1_VOICE | - |
| 210 | IDF2_DATA | - |
| 220 | IDF2_VOICE | - |
| 310 | IDF3_DATA | - |
| 320 | IDF3_VOICE | - |
| 4093 | MLAG_L3 | MLAG |
| 4094 | MLAG | MLAG |

### VLANs Device Configuration

```eos
!
vlan 110
   name IDF1_DATA
!
vlan 120
   name IDF1_VOICE
!
vlan 210
   name IDF2_DATA
!
vlan 220
   name IDF2_VOICE
!
vlan 310
   name IDF3_DATA
!
vlan 320
   name IDF3_VOICE
!
vlan 4093
   name MLAG_L3
   trunk group MLAG
!
vlan 4094
   name MLAG
   trunk group MLAG
```

## Interfaces

### Ethernet Interfaces

#### Ethernet Interfaces Summary

##### L2

| Interface | Description | Mode | VLANs | Native VLAN | Trunk Group | Channel-Group |
| --------- | ----------- | ---- | ----- | ----------- | ----------- | ------------- |
| Ethernet3 | L2_leaf-1a_Ethernet49 | *trunk | *110,120 | *- | *- | 3 |
| Ethernet4 | L2_leaf-2a_Ethernet1/1 | *trunk | *210,220 | *- | *- | 4 |
| Ethernet5 | L2_leaf-3a_Ethernet49 | *trunk | *310,320 | *- | *- | 5 |
| Ethernet6 | L2_leaf-3b_Ethernet49 | *trunk | *310,320 | *- | *- | 5 |
| Ethernet49/1 | MLAG_spine-2_Ethernet49/1 | *trunk | *- | *- | *MLAG | 491 |
| Ethernet50/1 | MLAG_spine-2_Ethernet50/1 | *trunk | *- | *- | *MLAG | 491 |

*Inherited from Port-Channel Interface

#### Ethernet Interfaces Device Configuration

```eos
!
interface Ethernet3
   description L2_leaf-1a_Ethernet49
   no shutdown
   channel-group 3 mode active
!
interface Ethernet4
   description L2_leaf-2a_Ethernet1/1
   no shutdown
   channel-group 4 mode active
!
interface Ethernet5
   description L2_leaf-3a_Ethernet49
   no shutdown
   channel-group 5 mode active
!
interface Ethernet6
   description L2_leaf-3b_Ethernet49
   no shutdown
   channel-group 5 mode active
!
interface Ethernet49/1
   description MLAG_spine-2_Ethernet49/1
   no shutdown
   channel-group 491 mode active
!
interface Ethernet50/1
   description MLAG_spine-2_Ethernet50/1
   no shutdown
   channel-group 491 mode active
```

### Port-Channel Interfaces

#### Port-Channel Interfaces Summary

##### L2

| Interface | Description | Mode | VLANs | Native VLAN | Trunk Group | LACP Fallback Timeout | LACP Fallback Mode | MLAG ID | EVPN ESI |
| --------- | ----------- | ---- | ----- | ----------- | ----------- | --------------------- | ------------------ | ------- | -------- |
| Port-Channel3 | L2_IDF1_Port-Channel49 | trunk | 110,120 | - | - | - | - | 3 | - |
| Port-Channel4 | L2_leaf-2a_Port-Channel11 | trunk | 210,220 | - | - | - | - | 4 | - |
| Port-Channel5 | L2_IDF3_Port-Channel49 | trunk | 310,320 | - | - | - | - | 5 | - |
| Port-Channel491 | MLAG_spine-2_Port-Channel491 | trunk | - | - | MLAG | - | - | - | - |

#### Port-Channel Interfaces Device Configuration

```eos
!
interface Port-Channel3
   description L2_IDF1_Port-Channel49
   no shutdown
   switchport trunk allowed vlan 110,120
   switchport mode trunk
   switchport
   mlag 3
!
interface Port-Channel4
   description L2_leaf-2a_Port-Channel11
   no shutdown
   switchport trunk allowed vlan 210,220
   switchport mode trunk
   switchport
   mlag 4
!
interface Port-Channel5
   description L2_IDF3_Port-Channel49
   no shutdown
   switchport trunk allowed vlan 310,320
   switchport mode trunk
   switchport
   mlag 5
!
interface Port-Channel491
   description MLAG_spine-2_Port-Channel491
   no shutdown
   switchport mode trunk
   switchport trunk group MLAG
   switchport
```

### Loopback Interfaces

#### Loopback Interfaces Summary

##### IPv4

| Interface | Description | VRF | IP Address |
| --------- | ----------- | --- | ---------- |
| Loopback0 | ROUTER_ID | default | 10.1.252.1/32 |

##### IPv6

| Interface | Description | VRF | IPv6 Addresses |
| --------- | ----------- | --- | -------------- |
| Loopback0 | ROUTER_ID | default | - |

#### Loopback Interfaces Device Configuration

```eos
!
interface Loopback0
   description ROUTER_ID
   no shutdown
   ip address 10.1.252.1/32
   ip ospf area 0.0.0.0
```

### VLAN Interfaces

#### VLAN Interfaces Summary

| Interface | Description | VRF | MTU | Shutdown |
| --------- | ----------- | --- | --- | -------- |
| Vlan110 | IDF1_DATA | default | - | False |
| Vlan120 | IDF1_VOICE | default | - | False |
| Vlan210 | IDF2_DATA | default | - | False |
| Vlan220 | IDF2_VOICE | default | - | False |
| Vlan310 | IDF3_DATA | default | - | False |
| Vlan320 | IDF3_VOICE | default | - | False |
| Vlan4093 | MLAG_L3 | default | 1500 | False |
| Vlan4094 | MLAG | default | 1500 | False |

##### IPv4

| Interface | VRF | IP Address | IP Address Virtual | IP Router Virtual Address | ACL In | ACL Out |
| --------- | --- | ---------- | ------------------ | ------------------------- | ------ | ------- |
| Vlan110 | default | 10.1.10.2/24 | - | 10.1.10.1 | - | - |
| Vlan120 | default | 10.1.20.2/24 | - | 10.1.20.1 | - | - |
| Vlan210 | default | 10.2.10.2/24 | - | 10.2.10.1 | - | - |
| Vlan220 | default | 10.2.20.2/24 | - | 10.2.20.1 | - | - |
| Vlan310 | default | 10.3.10.2/24 | - | 10.3.10.1 | - | - |
| Vlan320 | default | 10.3.20.2/24 | - | 10.3.20.1 | - | - |
| Vlan4093 | default | 10.1.253.2/31 | - | - | - | - |
| Vlan4094 | default | 10.1.253.0/31 | - | - | - | - |

##### OSPF

| Interface | OSPF Network Point to Point | OSPF Area | OSPF Cost | OSPF Authentication | IPv6 OSPF Process ID | IPv6 OSPF Area | IPv6 OSPF Network Point to Point |
| --------- | --------------------------- | --------- | --------- | ------------------- | -------------------- | -------------- | -------------------------------- |
| Vlan4093 | True | 0.0.0.0 | - | - | - | - | - |

#### VLAN Interfaces Device Configuration

```eos
!
interface Vlan110
   description IDF1_DATA
   no shutdown
   ip address 10.1.10.2/24
   ip virtual-router address 10.1.10.1
!
interface Vlan120
   description IDF1_VOICE
   no shutdown
   ip address 10.1.20.2/24
   ip virtual-router address 10.1.20.1
!
interface Vlan210
   description IDF2_DATA
   no shutdown
   ip address 10.2.10.2/24
   ip virtual-router address 10.2.10.1
!
interface Vlan220
   description IDF2_VOICE
   no shutdown
   ip address 10.2.20.2/24
   ip virtual-router address 10.2.20.1
!
interface Vlan310
   description IDF3_DATA
   no shutdown
   ip address 10.3.10.2/24
   ip virtual-router address 10.3.10.1
!
interface Vlan320
   description IDF3_VOICE
   no shutdown
   ip address 10.3.20.2/24
   ip virtual-router address 10.3.20.1
!
interface Vlan4093
   description MLAG_L3
   no shutdown
   mtu 1500
   ip address 10.1.253.2/31
   ip ospf network point-to-point
   ip ospf area 0.0.0.0
!
interface Vlan4094
   description MLAG
   no shutdown
   mtu 1500
   no autostate
   ip address 10.1.253.0/31
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

Virtual Router MAC Address: 00:1c:73:00:dc:01

#### Virtual Router MAC Address Device Configuration

```eos
!
ip virtual-router mac-address 00:1c:73:00:dc:01
```

### IP Routing

#### IP Routing Summary

| VRF | Routing Enabled |
| --- | --------------- |
| default | True |

#### IP Routing Device Configuration

```eos
!
ip routing
```

### IPv6 Routing

#### IPv6 Routing Summary

| VRF | Routing Enabled |
| --- | --------------- |
| default | False |
| default | false |

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

### Router OSPF

#### Router OSPF Summary

| Process ID | Router ID | Default Passive Interface | No Passive Interface | BFD | Max LSA | Default Information Originate | Log Adjacency Changes Detail | Auto Cost Reference Bandwidth | Maximum Paths | MPLS LDP Sync Default | Distribute List In |
| ---------- | --------- | ------------------------- | -------------------- | --- | ------- | ----------------------------- | ---------------------------- | ----------------------------- | ------------- | --------------------- | ------------------ |
| 100 | 10.1.252.1 | enabled | Vlan4093 | disabled | 12000 | disabled | disabled | - | - | - | - |

#### Router OSPF Router Redistribution

| Process ID | Source Protocol | Include Leaked | Route Map |
| ---------- | --------------- | -------------- | --------- |
| 100 | connected | disabled | - |

#### OSPF Interfaces

| Interface | Area | Cost | Point To Point |
| -------- | -------- | -------- | -------- |
| Vlan4093 | 0.0.0.0 | - | True |
| Loopback0 | 0.0.0.0 | - | - |

#### Router OSPF Device Configuration

```eos
!
router ospf 100
   router-id 10.1.252.1
   passive-interface default
   no passive-interface Vlan4093
   redistribute connected
   max-lsa 12000
   graceful-restart
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

## VRF Instances

### VRF Instances Summary

| VRF Name | IP Routing |
| -------- | ---------- |

### VRF Instances Device Configuration

```eos
```
