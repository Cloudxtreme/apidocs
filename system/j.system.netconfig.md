## j.system.netconfig

- /opt/jumpscale7/lib/JumpScale/baselib/netconfig/Netconfig.py
- Properties
    - root

    

### def reset(shutdown=False) (l51)

empty config of /etc/network/interfaces

### def shutdownNetwork(excludes=[]) (l25)

find all interfaces and shut them all down with ifdown
this is to remove all networking things going on

### def enableInterfaceBridge(dev,bridgedev,start=False,dhcp=True) (l188)

### def addIpToInterface(dev,ipaddr,aliasnr=1,start=False) (l205)

### def remove(dev) (l92)

### def enableInterfaceStatic(dev,ipaddr,gw=None,start=False) (l123)

ipaddr in form of 192.168.10.2/24 (can be list)
gateway in form of 192.168.10.254

### def setHostname(hostname) (l113)

change hostname

### def enableInterfaceBridgeStatic(dev,ipaddr=None,bridgedev=None,gw=None,start=False) (l143)

ipaddr in form of 192.168.10.2/24 (can be list)
gateway in form of 192.168.10.254

### def enableInterface(dev="eth0",start=False,dhcp=True) (l62)

### def enableInterfaceBridgeDhcp(dev,bridgedev,start=False) (l185)

### def setNameserver(addr) (l99)

resolvconf will be disabled

### def setRoot(root) (l17)

