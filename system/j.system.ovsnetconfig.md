## j.system.ovsnetconfig

- /opt/jumpscale7/lib/JumpScale/lib/ovsnetconfig/NetConfigFactory.py
- Properties
    - PHYSMTU

### Methods

#### applyconfig 
##### arguments

    - interfacenameToExclude
    - backplanename

##### comments

DANGEROUS, will remove old configuration

#### configureStaticAddress 
##### arguments

    - interfacename = 'eth0'
    - ipaddr = '192.168.10.10/24'
    - gw

##### comments

Configure a static address

#### createVXLanBridge 
##### arguments

    - networkid
    - backend
    - bridgename

##### comments

Creates a proper vxlan interface and bridge based on a backplane

#### ensureVXNet 
##### arguments

    - networkid
    - backend

##### comments

#### getConfigFromSystem 
##### arguments

    - reload = False

##### comments

walk over system and get configuration, result is dict

#### getType 
##### arguments

    - interfaceName

##### comments

#### initNetworkInterfaces 
##### arguments

##### comments

Resets /etc/network/interfaces with a basic configuration

#### newBondedBackplane 
##### arguments

    - name
    - interfaces
    - trunks

##### comments

Reasonable defaults  : mode=balance-tcp, lacp=active,fast, bondname=brname-Bond, all vlans allowed

#### newBridge 
##### arguments

    - name
    - interface

##### comments

@param interface interface where to connect this bridge to

#### newVlanBridge 
##### arguments

    - name
    - parentbridge
    - vlanid
    - mtu

##### comments

#### printConfigFromSystem 
##### arguments

##### comments

#### removeOldConfig 
##### arguments

##### comments

#### setBackplane 
##### arguments

    - interfacename = 'eth0'
    - backplanename = 1
    - ipaddr = '192.168.10.10/24'
    - gw = ''

##### comments

DANGEROUS, will remove old configuration

#### setBackplaneDhcp 
##### arguments

    - interfacename = 'eth0'
    - backplanename = 'Public'

##### comments

DANGEROUS, will remove old configuration

#### setBackplaneNoAddress 
##### arguments

    - interfacename = 'eth0'
    - backplanename = 1

##### comments

DANGEROUS, will remove old configuration

#### setBackplaneNoAddressWithBond 
##### arguments

    - bondname
    - bondinterfaces
    - backplanename = 'backplane'

##### comments

DANGEROUS, will remove old configuration

#### setBackplaneWithBond 
##### arguments

    - bondname
    - bondinterfaces
    - backplanename = 'backplane'
    - ipaddr = '192.168.10.10/24'
    - gw = ''

##### comments

DANGEROUS, will remove old configuration

