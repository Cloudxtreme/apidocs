## j.system.netconfig

- /opt/jumpscale7/lib/JumpScale/baselib/netconfig/Netconfig.py
- Properties
    - root

### Methods

    

#### addIpToInterface 
##### arguments

    - dev
    - ipaddr
    - aliasnr = 1
    - start = False

##### comments

#### enableInterface 
##### arguments

    - dev = 'eth0'
    - start = False
    - dhcp = True

##### comments

#### enableInterfaceBridge 
##### arguments

    - dev
    - bridgedev
    - start = False
    - dhcp = True

##### comments

#### enableInterfaceBridgeDhcp 
##### arguments

    - dev
    - bridgedev
    - start = False

##### comments

#### enableInterfaceBridgeStatic 
##### arguments

    - dev
    - ipaddr
    - bridgedev
    - gw
    - start = False

##### comments

ipaddr in form of 192.168.10.2/24 (can be list)
gateway in form of 192.168.10.254

#### enableInterfaceStatic 
##### arguments

    - dev
    - ipaddr
    - gw
    - start = False

##### comments

ipaddr in form of 192.168.10.2/24 (can be list)
gateway in form of 192.168.10.254

#### remove 
##### arguments

    - dev

##### comments

#### reset 
##### arguments

    - shutdown = False

##### comments

empty config of /etc/network/interfaces

#### setHostname 
##### arguments

    - hostname

##### comments

change hostname

#### setNameserver 
##### arguments

    - addr

##### comments

resolvconf will be disabled

#### setRoot 
##### arguments

    - root

##### comments

#### shutdownNetwork 
##### arguments

    - excludes = []

##### comments

find all interfaces and shut them all down with ifdown
this is to remove all networking things going on

