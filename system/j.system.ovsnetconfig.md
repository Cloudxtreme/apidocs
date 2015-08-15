## j.system.ovsnetconfig

- /opt/jumpscale7/lib/JumpScale/lib/ovsnetconfig/NetConfigFactory.py
- Properties
    - PHYSMTU

### Methods

#### def applyconfig 
##### arguments

- interfacenameToExclude
- backplanename

##### comments

```
DANGEROUS, will remove old configuration

```

#### def configureStaticAddress 
##### arguments

- interfacename = 'eth0'
- ipaddr = '192.168.10.10/24'
- gw

##### comments

```
Configure a static address

```

#### def createVXLanBridge 
##### arguments

- networkid
- backend
- bridgename

##### comments

```
Creates a proper vxlan interface and bridge based on a backplane

```

#### def ensureVXNet 
##### arguments

- networkid
- backend
#### def getConfigFromSystem 
##### arguments

- reload = False

##### comments

```
walk over system and get configuration, result is dict

```

#### def getType 
##### arguments

- interfaceName
#### def initNetworkInterfaces 
##### arguments

##### comments

```
Resets /etc/network/interfaces with a basic configuration

```

#### def newBondedBackplane 
##### arguments

- name
- interfaces
- trunks

##### comments

```
Reasonable defaults  : mode=balance-tcp, lacp=active,fast, bondname=brname-Bond, all vlans allowed

```

#### def newBridge 
##### arguments

- name
- interface

##### comments

```
@param interface interface where to connect this bridge to

```

#### def newVlanBridge 
##### arguments

- name
- parentbridge
- vlanid
- mtu
#### def printConfigFromSystem 
##### arguments

#### def removeOldConfig 
##### arguments

#### def setBackplane 
##### arguments

- interfacename = 'eth0'
- backplanename = 1
- ipaddr = '192.168.10.10/24'
- gw = ''

##### comments

```
DANGEROUS, will remove old configuration

```

#### def setBackplaneDhcp 
##### arguments

- interfacename = 'eth0'
- backplanename = 'Public'

##### comments

```
DANGEROUS, will remove old configuration

```

#### def setBackplaneNoAddress 
##### arguments

- interfacename = 'eth0'
- backplanename = 1

##### comments

```
DANGEROUS, will remove old configuration

```

#### def setBackplaneNoAddressWithBond 
##### arguments

- bondname
- bondinterfaces
- backplanename = 'backplane'

##### comments

```
DANGEROUS, will remove old configuration

```

#### def setBackplaneWithBond 
##### arguments

- bondname
- bondinterfaces
- backplanename = 'backplane'
- ipaddr = '192.168.10.10/24'
- gw = ''

##### comments

```
DANGEROUS, will remove old configuration

```

