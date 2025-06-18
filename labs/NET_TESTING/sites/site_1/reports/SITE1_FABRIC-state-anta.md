# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed | Total Tests Skipped |
| ----------- | ------------------ | ------------------ | ------------------- |
| 398 | 358 | 8 | 32 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| s1-brdr1 | 53 | 48 | 1 | 4 | System | Hardware |
| s1-brdr2 | 53 | 48 | 1 | 4 | System | Hardware |
| s1-leaf1 | 54 | 49 | 1 | 4 | System | Hardware |
| s1-leaf2 | 54 | 49 | 1 | 4 | System | Hardware |
| s1-leaf3 | 54 | 49 | 1 | 4 | System | Hardware |
| s1-leaf4 | 54 | 49 | 1 | 4 | System | Hardware |
| s1-spine1 | 38 | 33 | 1 | 4 | System | Hardware |
| s1-spine2 | 38 | 33 | 1 | 4 | System | Hardware |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| BGP | 54 | 54 | 0 | 0 |
| Connectivity | 108 | 108 | 0 | 0 |
| Hardware | 32 | 0 | 0 | 32 |
| Interfaces | 108 | 108 | 0 | 0 |
| MLAG | 6 | 6 | 0 | 0 |
| Routing | 74 | 74 | 0 | 0 |
| System | 16 | 8 | 8 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 53 | s1-brdr1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 106 | s1-brdr2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 160 | s1-leaf1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 214 | s1-leaf2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 268 | s1-leaf3 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 322 | s1-leaf4 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 360 | s1-spine1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 398 | s1-spine2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 2 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 3 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr2 (IP: 10.252.1.9) | PASS | - |
| 4 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.16) | PASS | - |
| 5 | s1-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.18) | PASS | - |
| 6 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-brdr2 Ethernet1 | PASS | - |
| 7 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet7 | PASS | - |
| 8 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet7 | PASS | - |
| 9 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-brdr2 Ethernet6 | PASS | - |
| 10 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 11 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 12 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 13 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 14 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 15 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 16 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 17 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.7) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 18 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.17) - Destination: s1-spine1 Ethernet7 (IP: 172.16.1.16) | PASS | - |
| 19 | s1-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.19) - Destination: s1-spine2 Ethernet7 (IP: 172.16.1.18) | PASS | - |
| 20 | s1-brdr1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 21 | s1-brdr1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 22 | s1-brdr1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 23 | s1-brdr1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 24 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-brdr2_Ethernet1 = 'up' | PASS | - |
| 25 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet7 = 'up' | PASS | - |
| 26 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet7 = 'up' | PASS | - |
| 27 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_s2-brdr1_Ethernet4 = 'up' | PASS | - |
| 28 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-brdr2_Ethernet6 = 'up' | PASS | - |
| 29 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 30 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 31 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-brdr2_Port-Channel1 = 'up' | PASS | - |
| 32 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 33 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 34 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 35 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 36 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 37 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 38 | s1-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 39 | s1-brdr1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 40 | s1-brdr1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 41 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 42 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 43 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 44 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 45 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 46 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 47 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 48 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 49 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 50 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 51 | s1-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 52 | s1-brdr1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 53 | s1-brdr1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 54 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 55 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 56 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr1 (IP: 10.252.1.8) | PASS | - |
| 57 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.20) | PASS | - |
| 58 | s1-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.22) | PASS | - |
| 59 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-brdr1 Ethernet1 | PASS | - |
| 60 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet8 | PASS | - |
| 61 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet8 | PASS | - |
| 62 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-brdr1 Ethernet6 | PASS | - |
| 63 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 64 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 65 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 66 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 67 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 68 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 69 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 70 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.8) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 71 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.21) - Destination: s1-spine1 Ethernet8 (IP: 172.16.1.20) | PASS | - |
| 72 | s1-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.23) - Destination: s1-spine2 Ethernet8 (IP: 172.16.1.22) | PASS | - |
| 73 | s1-brdr2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 74 | s1-brdr2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 75 | s1-brdr2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 76 | s1-brdr2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 77 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-brdr1_Ethernet1 = 'up' | PASS | - |
| 78 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet8 = 'up' | PASS | - |
| 79 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet8 = 'up' | PASS | - |
| 80 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_s2-brdr2_Ethernet5 = 'up' | PASS | - |
| 81 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-brdr1_Ethernet6 = 'up' | PASS | - |
| 82 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 83 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 84 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-brdr1_Port-Channel1 = 'up' | PASS | - |
| 85 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 86 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 87 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 88 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 89 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 90 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 91 | s1-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 92 | s1-brdr2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 93 | s1-brdr2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 94 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 95 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 96 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 97 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 98 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 99 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 100 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 101 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 102 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 103 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 104 | s1-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 105 | s1-brdr2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 106 | s1-brdr2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 107 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 108 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 109 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf2 (IP: 10.252.1.1) | PASS | - |
| 110 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.0) | PASS | - |
| 111 | s1-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.2) | PASS | - |
| 112 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-leaf2 Ethernet1 | PASS | - |
| 113 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet2 | PASS | - |
| 114 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet2 | PASS | - |
| 115 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-leaf2 Ethernet6 | PASS | - |
| 116 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 117 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 118 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 119 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 120 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 121 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 122 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 123 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.3) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 124 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.1) - Destination: s1-spine1 Ethernet2 (IP: 172.16.1.0) | PASS | - |
| 125 | s1-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.3) - Destination: s1-spine2 Ethernet2 (IP: 172.16.1.2) | PASS | - |
| 126 | s1-leaf1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 127 | s1-leaf1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 128 | s1-leaf1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 129 | s1-leaf1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 130 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-leaf2_Ethernet1 = 'up' | PASS | - |
| 131 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet2 = 'up' | PASS | - |
| 132 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet2 = 'up' | PASS | - |
| 133 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s1-host1_eth1 = 'up' | PASS | - |
| 134 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-leaf2_Ethernet6 = 'up' | PASS | - |
| 135 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 136 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 137 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-leaf2_Port-Channel1 = 'up' | PASS | - |
| 138 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s1-host1 = 'up' | PASS | - |
| 139 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 140 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 141 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 142 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 143 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 144 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 145 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 146 | s1-leaf1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 147 | s1-leaf1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 148 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 149 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 150 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 151 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 152 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 153 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 154 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 155 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 156 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 157 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 158 | s1-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 159 | s1-leaf1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 160 | s1-leaf1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 161 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 162 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 163 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf1 (IP: 10.252.1.0) | PASS | - |
| 164 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.4) | PASS | - |
| 165 | s1-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.6) | PASS | - |
| 166 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-leaf1 Ethernet1 | PASS | - |
| 167 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet3 | PASS | - |
| 168 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet3 | PASS | - |
| 169 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-leaf1 Ethernet6 | PASS | - |
| 170 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 171 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 172 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 173 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 174 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 175 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 176 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 177 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.4) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 178 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.5) - Destination: s1-spine1 Ethernet3 (IP: 172.16.1.4) | PASS | - |
| 179 | s1-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.7) - Destination: s1-spine2 Ethernet3 (IP: 172.16.1.6) | PASS | - |
| 180 | s1-leaf2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 181 | s1-leaf2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 182 | s1-leaf2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 183 | s1-leaf2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 184 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-leaf1_Ethernet1 = 'up' | PASS | - |
| 185 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet3 = 'up' | PASS | - |
| 186 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet3 = 'up' | PASS | - |
| 187 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s1-host1_eth2 = 'up' | PASS | - |
| 188 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-leaf1_Ethernet6 = 'up' | PASS | - |
| 189 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 190 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 191 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-leaf1_Port-Channel1 = 'up' | PASS | - |
| 192 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s1-host1 = 'up' | PASS | - |
| 193 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 194 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 195 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 196 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 197 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 198 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 199 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 200 | s1-leaf2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 201 | s1-leaf2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 202 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 203 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 204 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 205 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 206 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 207 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 208 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 209 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 210 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 211 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 212 | s1-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 213 | s1-leaf2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 214 | s1-leaf2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 215 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 216 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 217 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf4 (IP: 10.252.1.5) | PASS | - |
| 218 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.8) | PASS | - |
| 219 | s1-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.10) | PASS | - |
| 220 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-leaf4 Ethernet1 | PASS | - |
| 221 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet4 | PASS | - |
| 222 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet4 | PASS | - |
| 223 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-leaf4 Ethernet6 | PASS | - |
| 224 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 225 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 226 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 227 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 228 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 229 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 230 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 231 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.5) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 232 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.9) - Destination: s1-spine1 Ethernet4 (IP: 172.16.1.8) | PASS | - |
| 233 | s1-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.11) - Destination: s1-spine2 Ethernet4 (IP: 172.16.1.10) | PASS | - |
| 234 | s1-leaf3 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 235 | s1-leaf3 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 236 | s1-leaf3 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 237 | s1-leaf3 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 238 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-leaf4_Ethernet1 = 'up' | PASS | - |
| 239 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet4 = 'up' | PASS | - |
| 240 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet4 = 'up' | PASS | - |
| 241 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s1-host2_eth1 = 'up' | PASS | - |
| 242 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-leaf4_Ethernet6 = 'up' | PASS | - |
| 243 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 244 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 245 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-leaf4_Port-Channel1 = 'up' | PASS | - |
| 246 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s1-host2 = 'up' | PASS | - |
| 247 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 248 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 249 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 250 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 251 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 252 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 253 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 254 | s1-leaf3 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 255 | s1-leaf3 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 256 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 257 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 258 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 259 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 260 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 261 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 262 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 263 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 264 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 265 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 266 | s1-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 267 | s1-leaf3 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 268 | s1-leaf3 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 269 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine1 (IP: 10.250.1.1) | PASS | - |
| 270 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-spine2 (IP: 10.250.1.2) | PASS | - |
| 271 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf3 (IP: 10.252.1.4) | PASS | - |
| 272 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine1 (IP: 172.16.1.12) | PASS | - |
| 273 | s1-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-spine2 (IP: 172.16.1.14) | PASS | - |
| 274 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-leaf3 Ethernet1 | PASS | - |
| 275 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-spine1 Ethernet5 | PASS | - |
| 276 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-spine2 Ethernet5 | PASS | - |
| 277 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-leaf3 Ethernet6 | PASS | - |
| 278 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-brdr1 Loopback0 (IP: 10.250.1.7) | PASS | - |
| 279 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-brdr2 Loopback0 (IP: 10.250.1.8) | PASS | - |
| 280 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-leaf1 Loopback0 (IP: 10.250.1.3) | PASS | - |
| 281 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-leaf2 Loopback0 (IP: 10.250.1.4) | PASS | - |
| 282 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-leaf3 Loopback0 (IP: 10.250.1.5) | PASS | - |
| 283 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-leaf4 Loopback0 (IP: 10.250.1.6) | PASS | - |
| 284 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-spine1 Loopback0 (IP: 10.250.1.1) | PASS | - |
| 285 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.1.6) - Destination: s1-spine2 Loopback0 (IP: 10.250.1.2) | PASS | - |
| 286 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.13) - Destination: s1-spine1 Ethernet5 (IP: 172.16.1.12) | PASS | - |
| 287 | s1-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.15) - Destination: s1-spine2 Ethernet5 (IP: 172.16.1.14) | PASS | - |
| 288 | s1-leaf4 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 289 | s1-leaf4 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 290 | s1-leaf4 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 291 | s1-leaf4 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 292 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-leaf3_Ethernet1 = 'up' | PASS | - |
| 293 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-spine1_Ethernet5 = 'up' | PASS | - |
| 294 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-spine2_Ethernet5 = 'up' | PASS | - |
| 295 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s1-host2_eth2 = 'up' | PASS | - |
| 296 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-leaf3_Ethernet6 = 'up' | PASS | - |
| 297 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 298 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 299 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-leaf3_Port-Channel1 = 'up' | PASS | - |
| 300 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s1-host2 = 'up' | PASS | - |
| 301 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 302 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 303 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan30 - Thiry = 'up' | PASS | - |
| 304 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 305 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 306 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 307 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 308 | s1-leaf4 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 309 | s1-leaf4 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 310 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.1 - Peer: s1-spine1 | PASS | - |
| 311 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.2 - Peer: s1-spine2 | PASS | - |
| 312 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.3 - Peer: s1-leaf1 | PASS | - |
| 313 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.4 - Peer: s1-leaf2 | PASS | - |
| 314 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.5 - Peer: s1-leaf3 | PASS | - |
| 315 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.6 - Peer: s1-leaf4 | PASS | - |
| 316 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.7 - Peer: s1-brdr1 | PASS | - |
| 317 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.1.8 - Peer: s1-brdr2 | PASS | - |
| 318 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: s1-leaf1 | PASS | - |
| 319 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: s1-leaf3 | PASS | - |
| 320 | s1-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.7 - Peer: s1-brdr1 | PASS | - |
| 321 | s1-leaf4 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 322 | s1-leaf4 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 323 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-brdr1 (IP: 10.250.1.7) | PASS | - |
| 324 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-brdr2 (IP: 10.250.1.8) | PASS | - |
| 325 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf1 (IP: 10.250.1.3) | PASS | - |
| 326 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf2 (IP: 10.250.1.4) | PASS | - |
| 327 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf3 (IP: 10.250.1.5) | PASS | - |
| 328 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf4 (IP: 10.250.1.6) | PASS | - |
| 329 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr1 (IP: 172.16.1.17) | PASS | - |
| 330 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr2 (IP: 172.16.1.21) | PASS | - |
| 331 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf1 (IP: 172.16.1.1) | PASS | - |
| 332 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf2 (IP: 172.16.1.5) | PASS | - |
| 333 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf3 (IP: 172.16.1.9) | PASS | - |
| 334 | s1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf4 (IP: 172.16.1.13) | PASS | - |
| 335 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-leaf1 Ethernet2 | PASS | - |
| 336 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-leaf2 Ethernet2 | PASS | - |
| 337 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: s1-leaf3 Ethernet2 | PASS | - |
| 338 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: s1-leaf4 Ethernet2 | PASS | - |
| 339 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet7 - Remote: s1-brdr1 Ethernet2 | PASS | - |
| 340 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet8 - Remote: s1-brdr2 Ethernet2 | PASS | - |
| 341 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.0) - Destination: s1-leaf1 Ethernet2 (IP: 172.16.1.1) | PASS | - |
| 342 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.4) - Destination: s1-leaf2 Ethernet2 (IP: 172.16.1.5) | PASS | - |
| 343 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4 (IP: 172.16.1.8) - Destination: s1-leaf3 Ethernet2 (IP: 172.16.1.9) | PASS | - |
| 344 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet5 (IP: 172.16.1.12) - Destination: s1-leaf4 Ethernet2 (IP: 172.16.1.13) | PASS | - |
| 345 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet7 (IP: 172.16.1.16) - Destination: s1-brdr1 Ethernet2 (IP: 172.16.1.17) | PASS | - |
| 346 | s1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet8 (IP: 172.16.1.20) - Destination: s1-brdr2 Ethernet2 (IP: 172.16.1.21) | PASS | - |
| 347 | s1-spine1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 348 | s1-spine1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 349 | s1-spine1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 350 | s1-spine1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 351 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-leaf1_Ethernet2 = 'up' | PASS | - |
| 352 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-leaf2_Ethernet2 = 'up' | PASS | - |
| 353 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_s1-leaf3_Ethernet2 = 'up' | PASS | - |
| 354 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_s1-leaf4_Ethernet2 = 'up' | PASS | - |
| 355 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet7 - P2P_s1-brdr1_Ethernet2 = 'up' | PASS | - |
| 356 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet8 - P2P_s1-brdr2_Ethernet2 = 'up' | PASS | - |
| 357 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 358 | s1-spine1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 359 | s1-spine1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 360 | s1-spine1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 361 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-brdr1 (IP: 10.250.1.7) | PASS | - |
| 362 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-brdr2 (IP: 10.250.1.8) | PASS | - |
| 363 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf1 (IP: 10.250.1.3) | PASS | - |
| 364 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf2 (IP: 10.250.1.4) | PASS | - |
| 365 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf3 (IP: 10.250.1.5) | PASS | - |
| 366 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s1-leaf4 (IP: 10.250.1.6) | PASS | - |
| 367 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr1 (IP: 172.16.1.19) | PASS | - |
| 368 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-brdr2 (IP: 172.16.1.23) | PASS | - |
| 369 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf1 (IP: 172.16.1.3) | PASS | - |
| 370 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf2 (IP: 172.16.1.7) | PASS | - |
| 371 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf3 (IP: 172.16.1.11) | PASS | - |
| 372 | s1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s1-leaf4 (IP: 172.16.1.15) | PASS | - |
| 373 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-leaf1 Ethernet3 | PASS | - |
| 374 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-leaf2 Ethernet3 | PASS | - |
| 375 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: s1-leaf3 Ethernet3 | PASS | - |
| 376 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: s1-leaf4 Ethernet3 | PASS | - |
| 377 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet7 - Remote: s1-brdr1 Ethernet3 | PASS | - |
| 378 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet8 - Remote: s1-brdr2 Ethernet3 | PASS | - |
| 379 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.1.2) - Destination: s1-leaf1 Ethernet3 (IP: 172.16.1.3) | PASS | - |
| 380 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.1.6) - Destination: s1-leaf2 Ethernet3 (IP: 172.16.1.7) | PASS | - |
| 381 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4 (IP: 172.16.1.10) - Destination: s1-leaf3 Ethernet3 (IP: 172.16.1.11) | PASS | - |
| 382 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet5 (IP: 172.16.1.14) - Destination: s1-leaf4 Ethernet3 (IP: 172.16.1.15) | PASS | - |
| 383 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet7 (IP: 172.16.1.18) - Destination: s1-brdr1 Ethernet3 (IP: 172.16.1.19) | PASS | - |
| 384 | s1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet8 (IP: 172.16.1.22) - Destination: s1-brdr2 Ethernet3 (IP: 172.16.1.23) | PASS | - |
| 385 | s1-spine2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 386 | s1-spine2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 387 | s1-spine2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 388 | s1-spine2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 389 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s1-leaf1_Ethernet3 = 'up' | PASS | - |
| 390 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s1-leaf2_Ethernet3 = 'up' | PASS | - |
| 391 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_s1-leaf3_Ethernet3 = 'up' | PASS | - |
| 392 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_s1-leaf4_Ethernet3 = 'up' | PASS | - |
| 393 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet7 - P2P_s1-brdr1_Ethernet3 = 'up' | PASS | - |
| 394 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet8 - P2P_s1-brdr2_Ethernet3 = 'up' | PASS | - |
| 395 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 396 | s1-spine2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 397 | s1-spine2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 398 | s1-spine2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
