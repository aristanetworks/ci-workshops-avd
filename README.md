# Arista CI Workshops

## Dual Datacenter Topology

Site 1

- vlan 10, 10.10.10.0/24
- vlan 20, 10.20.20.0/24

Site 2

- vlan 30, 10.30.30.0/24
- vlan 40, 10.40.40.0/24

![ATD L2LS Topo](images/atd-avd-dual-dc-l2ls-topo.png)

## Create ATD Lab

Create a new ATD Dual Center Lab and then follow along
## Clone this repo to ATD Programmability IDE

``` bash
cd /home/coder/project/labfiles
git clone https://github.com/mthiel117/atd-avd-dual-dc-l2ls.git
```

## ATD Lab Updates

Update AVD to latest version

``` bash
ansible-galaxy collection install arista.avd --force
```

Install Deepmerge module

``` bash
pip install deepmerge
```

## Initialize WAN environment

Push pre-defined configs for WAN Nodes

``` bash
make prepwan
```

## Update Passwords & SSH in Data Models

>Note: Needs work to make this easier...  Eliminate the need to manually gen sha512 password and populate Lab password across multiple files...

- sites/site_2/group_vars/SITE2.yml (line 4)
- sites/site_2/group_vars/SITE2.yml (line 4)
- wan_configs/group_vars/WAN.yml (line 4)
- global_vars/global_dc_vars.yml (line 34-35)

## Build Site Configs

``` bash
# Build Site 1 Configs
make build-site-1

# Build Site 2 Configs
make build-site-2
```

## Deploy Site Configs

``` bash
# Build Site 1 Configs
make deploy-site-1

# Build Site 2 Configs
make deploy-site-2
```

## Test Traffic

Log on to a a spine a look at OSPF neighbors and ip routes.  Ping across to the the side.

From s1-spine1

``` bash
show ip ospf neighbors

show ip route

ping 10.30.30.1
```