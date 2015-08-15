<!-- toc -->
## j.ssh.ubuntu.NetworkManager

- /opt/jumpscale7/lib/JumpScale/lib/ssh/ubuntu/manager.py

### Methods

#### def commit 

##### arguments

- device

#### def ipGet 

##### arguments

- device

##### comments

```
Get IP of devie
Result (ip, netmask, gateway)

```

#### def ipReset 

##### arguments

- device
- commit = False

#### def ipSet 

##### arguments

- device
- ip
- netmask
- gw
- inet = 'dhcp'
- commit = False

##### comments

```
Return all interfaces that has this ifname

```

#### def nsGet 

##### arguments

#### def nsSet 

##### arguments

- nameservers = []
- commit = False

#### def setHostname 

##### arguments

- hostname

