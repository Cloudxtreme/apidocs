## j.system.ovsnetconfig

- /opt/jumpscale7/lib/JumpScale/lib/ovsnetconfig/NetConfigFactory.py
- Properties
    - PHYSMTU

### def newBondedBackplane(name, interfaces, trunks=None) (l337)

Reasonable defaults  : mode=balance-tcp, lacp=active,fast, bondname=brname-Bond, all vlans allowed

### def newVlanBridge(name, parentbridge, vlanid, mtu=None) (l89)

### def setBackplaneNoAddressWithBond(bondname, bondinterfaces,backplanename='backplane') (l196)

DANGEROUS, will remove old configuration

### def setBackplaneWithBond(bondname, bondinterfaces,backplanename='backplane',ipaddr="192.168.10.10/24",gw="") (l269)

DANGEROUS, will remove old configuration

### def printConfigFromSystem() (l77)

### def removeOldConfig() (l34)

### def getType(interfaceName) (l112)

### def setBackplaneDhcp(interfacename="eth0",backplanename="Public") (l121)

DANGEROUS, will remove old configuration

### def applyconfig(interfacenameToExclude=None,backplanename=None) (l315)

DANGEROUS, will remove old configuration

### def setBackplaneNoAddress(interfacename="eth0",backplanename=1) (l146)

DANGEROUS, will remove old configuration

### def configureStaticAddress(interfacename="eth0",ipaddr="192.168.10.10/24",gw=None) (l169)

Configure a static address

### def createVXLanBridge(networkid, backend,bridgename=None) (l99)

Creates a proper vxlan interface and bridge based on a backplane

### def newBridge(name,interface=None) (l80)

@param interface interface where to connect this bridge to

### def initNetworkInterfaces() (l71)

Resets /etc/network/interfaces with a basic configuration

### def getConfigFromSystem(reload=False) (l19)

walk over system and get configuration, result is dict

### def ensureVXNet(networkid, backend) (l92)

### def setBackplane(interfacename="eth0",backplanename=1,ipaddr="192.168.10.10/24",gw="") (l233)

DANGEROUS, will remove old configuration

