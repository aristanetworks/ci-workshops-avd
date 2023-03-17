# Arista CI Workshops

## Dual Datacenter Topology

### Site Vlans and Subnets

| Site | Vlan |     Subnet    |
|:----:|:----:|:-------------:|
| 1    | 10   | 10.10.10.0/24 |
| 1    | 20   | 10.20.20.0/24 |
| 2    | 30   | 10.30.30.0/24 |
| 2    | 40   | 10.40.40.0/24 |

### Host Addressing

| Site | Rack | Hostname | IP Address.     |
|:----:|:----:|:--------:|:---------------:|
| 1    | 1    | s1-host1 | 10.10.10.100/24 |
| 1    | 2    | s1-host2 | 10.20.20.100/24 |
| 2    | 1    | s2-host1 | 10.30.30.100/24 |
| 2    | 2    | s2-host2 | 10.40.40.100/24 |

### WAN - IP Network

The WAN IP Network runs OSPF in Area 0.0.0.0 using /31's in the 10.0.0.0/24 address block.  The Spines in each DC will peer to nodes in the cloud.

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

## Set Lab Password environment variable

The following command sets the environment variable `LABPASSPHRASE` which is used later for connecting to your lab switches and creating local user password.

``` bash
export LABPASSPHRASE=`cat /home/coder/.config/code-server/config.yaml| grep "password:" | awk '{print $2}'
```

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

Log on to a spine to verify OSPF neighbors and ip routes.

From `s1-spine1`

``` bash
show ip ospf neighbors
show ip route
ping 10.30.30.1
```

Log on to a host and ping to a remote host.

From `s1-host1` ping `s2-host2`.

``` bash
ping 10.40.40.100
```