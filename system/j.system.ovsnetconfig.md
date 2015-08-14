## j.system.ovsnetconfig

- /opt/jumpscale7/lib/JumpScale/lib/ovsnetconfig/NetConfigFactory.py
- Properties
    - PHYSMTU

    #### def applyconfig(interfacenameToExclude=None,backplanename=None) 
    
    DANGEROUS, will remove old configuration
    #### def configureStaticAddress(interfacename="eth0",ipaddr="192.168.10.10/24",gw=None) 
    
    Configure a static address
    #### def createVXLanBridge(networkid, backend,bridgename=None) 
    
    Creates a proper vxlan interface and bridge based on a backplane
    #### def ensureVXNet(networkid, backend) 
    #### def getConfigFromSystem(reload=False) 
    
    walk over system and get configuration, result is dict
    #### def getType(interfaceName) 
    #### def initNetworkInterfaces() 
    
    Resets /etc/network/interfaces with a basic configuration
    #### def newBondedBackplane(name, interfaces, trunks=None) 
    
    Reasonable defaults  : mode=balance-tcp, lacp=active,fast, bondname=brname-Bond, all vlans allowed
    #### def newBridge(name,interface=None) 
    
    @param interface interface where to connect this bridge to
    #### def newVlanBridge(name, parentbridge, vlanid, mtu=None) 
    #### def printConfigFromSystem() 
    #### def removeOldConfig() 
    #### def setBackplane(interfacename="eth0",backplanename=1,ipaddr="192.168.10.10/24",gw="") 
    
    DANGEROUS, will remove old configuration
    #### def setBackplaneDhcp(interfacename="eth0",backplanename="Public") 
    
    DANGEROUS, will remove old configuration
    #### def setBackplaneNoAddress(interfacename="eth0",backplanename=1) 
    
    DANGEROUS, will remove old configuration
    #### def setBackplaneNoAddressWithBond(bondname, bondinterfaces,backplanename='backplane') 
    
    DANGEROUS, will remove old configuration
    #### def setBackplaneWithBond(bondname, bondinterfaces,backplanename='backplane',ipaddr="192.168.10.10/24",gw="") 
    
    DANGEROUS, will remove old configuration
