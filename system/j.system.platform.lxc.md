## j.system.platform.lxc

- /opt/jumpscale7/lib/JumpScale/lib/lxc/Lxc.py

### Methods

#### def btrfsSubvolCopy 

##### arguments

- nameFrom
- NameDest

#### def btrfsSubvolDelete 

##### arguments

- name

#### def btrfsSubvolExists 

##### arguments

- name

#### def btrfsSubvolList 

##### arguments

#### def btrfsSubvolNew 

##### arguments

- name

#### def create 

##### arguments

- name = ''
- stdout = True
- base = 'base'
- start = False
- nameserver = '8.8.8.8'
- replace = True

##### comments

```
@param name if "" then will be an incremental nr

```

#### def destroy 

##### arguments

- name

#### def destroyAll 

##### arguments

#### def execute 

##### arguments

- command

#### def exportRsync 

##### arguments

- name
- backupname
- key = 'pub'

#### def exportTgz 

##### arguments

- name
- backupname

#### def getConfig 

##### arguments

- name

#### def getIp 

##### arguments

- name
- fail = True

#### def getPid 

##### arguments

- name
- fail = True

#### def getProcessList 

##### arguments

- name
- stdout = True

##### comments

```
@return [["$name",$pid,$mem,$parent],....,[$mem,$cpu]]
last one is sum of mem & cpu

```

#### def importRsync 

##### arguments

- backupname
- name
- basename = ''
- key = 'pub'

##### comments

```
@param basename is the name of a start of a machine locally, will be used as
    basis and then the source will be synced over it

```

#### def importTgz 

##### arguments

- backupname
- name

#### def list 

##### arguments

##### comments

```
names of running & stopped machines
@return (running,stopped)

```

#### def networkSet 

##### arguments

- machinename
- netname = 'pub0'
- pubips = []
- bridge = 'public'
- gateway

#### def networkSetPrivateVXLan 

##### arguments

- name
- vxlanid
- ipaddresses

#### def pushSSHKey 

##### arguments

- name

#### def removeRedundantFiles 

##### arguments

- name

#### def setHostName 

##### arguments

- name

#### def start 

##### arguments

- name
- stdout = True
- test = True

#### def stop 

##### arguments

- name

