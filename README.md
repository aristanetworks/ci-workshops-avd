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
git clone https://github.com/PacketAnglers/workshops-avd.git
cd workshops-avd
```

## ATD Lab Updates

Update AVD and requirements to the latest version

``` bash
ansible-galaxy collection install arista.avd arista.cvp --force
export ARISTA_AVD_DIR=$(ansible-galaxy collection list arista.avd --format yaml | head -1 | cut -d: -f1)
pip3 config set global.disable-pip-version-check true
pip3 install -r ${ARISTA_AVD_DIR}/arista/avd/requirements.txt
```

## Update Password in Global Vars

Update `ansible_password:` in global_vars/global_dc_vars.yml (line 5).

## Initialize WAN environment

Push pre-defined configs for WAN & Host Nodes

``` bash
make preplab
```

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
