## j.system.netconfig

- /opt/jumpscale7/lib/JumpScale/baselib/netconfig/Netconfig.py
- Properties
    - root

    

    #### def addIpToInterface(dev,ipaddr,aliasnr=1,start=False) 
    #### def enableInterface(dev="eth0",start=False,dhcp=True) 
    #### def enableInterfaceBridge(dev,bridgedev,start=False,dhcp=True) 
    #### def enableInterfaceBridgeDhcp(dev,bridgedev,start=False) 
    #### def enableInterfaceBridgeStatic(dev,ipaddr=None,bridgedev=None,gw=None,start=False) 
    
    ipaddr in form of 192.168.10.2/24 (can be list)
    gateway in form of 192.168.10.254
    #### def enableInterfaceStatic(dev,ipaddr,gw=None,start=False) 
    
    ipaddr in form of 192.168.10.2/24 (can be list)
    gateway in form of 192.168.10.254
    #### def remove(dev) 
    #### def reset(shutdown=False) 
    
    empty config of /etc/network/interfaces
    #### def setHostname(hostname) 
    
    change hostname
    #### def setNameserver(addr) 
    
    resolvconf will be disabled
    #### def setRoot(root) 
    #### def shutdownNetwork(excludes=[]) 
    
    find all interfaces and shut them all down with ifdown
    this is to remove all networking things going on
