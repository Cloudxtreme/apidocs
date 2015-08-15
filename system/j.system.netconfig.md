## j.system.netconfig

- /opt/jumpscale7/lib/JumpScale/baselib/netconfig/Netconfig.py
- Properties
    - root

### Methods

    

#### def addIpToInterface 

##### arguments

- dev
- ipaddr
- aliasnr = 1
- start = False

#### def enableInterface 

##### arguments

- dev = 'eth0'
- start = False
- dhcp = True

#### def enableInterfaceBridge 

##### arguments

- dev
- bridgedev
- start = False
- dhcp = True

#### def enableInterfaceBridgeDhcp 

##### arguments

- dev
- bridgedev
- start = False

#### def enableInterfaceBridgeStatic 

##### arguments

- dev
- ipaddr
- bridgedev
- gw
- start = False

##### comments

```
ipaddr in form of 192.168.10.2/24 (can be list)
gateway in form of 192.168.10.254

```

#### def enableInterfaceStatic 

##### arguments

- dev
- ipaddr
- gw
- start = False

##### comments

```
ipaddr in form of 192.168.10.2/24 (can be list)
gateway in form of 192.168.10.254

```

#### def remove 

##### arguments

- dev

#### def reset 

##### arguments

- shutdown = False

##### comments

```
empty config of /etc/network/interfaces

```

#### def setHostname 

##### arguments

- hostname

##### comments

```
change hostname

```

#### def setNameserver 

##### arguments

- addr

##### comments

```
resolvconf will be disabled

```

#### def setRoot 

##### arguments

- root

#### def shutdownNetwork 

##### arguments

- excludes = []

##### comments

```
find all interfaces and shut them all down with ifdown
this is to remove all networking things going on

```

