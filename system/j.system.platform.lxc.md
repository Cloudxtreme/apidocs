## j.system.platform.lxc

- /opt/jumpscale7/lib/JumpScale/lib/lxc/Lxc.py

### Methods

#### def btrfsSubvolCopy 
##### arguments

- nameFrom
- NameDest

##### comments

```

```

#### def btrfsSubvolDelete 
##### arguments

- name

##### comments

```

```

#### def btrfsSubvolExists 
##### arguments

- name

##### comments

```

```

#### def btrfsSubvolList 
##### arguments

##### comments

```

```

#### def btrfsSubvolNew 
##### arguments

- name

##### comments

```

```

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

##### comments

```

```

#### def destroyAll 
##### arguments

##### comments

```

```

#### def execute 
##### arguments

- command

##### comments

```

```

#### def exportRsync 
##### arguments

- name
- backupname
- key = 'pub'

##### comments

```

```

#### def exportTgz 
##### arguments

- name
- backupname

##### comments

```

```

#### def getConfig 
##### arguments

- name

##### comments

```

```

#### def getIp 
##### arguments

- name
- fail = True

##### comments

```

```

#### def getPid 
##### arguments

- name
- fail = True

##### comments

```

```

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
@param basename is the name of a start of a machine locally, will be used as basis and then the source will be synced over it

```

#### def importTgz 
##### arguments

- backupname
- name

##### comments

```

```

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

##### comments

```

```

#### def networkSetPrivateVXLan 
##### arguments

- name
- vxlanid
- ipaddresses

##### comments

```

```

#### def pushSSHKey 
##### arguments

- name

##### comments

```

```

#### def removeRedundantFiles 
##### arguments

- name

##### comments

```

```

#### def setHostName 
##### arguments

- name

##### comments

```

```

#### def start 
##### arguments

- name
- stdout = True
- test = True

##### comments

```

```

#### def stop 
##### arguments

- name

##### comments

```

```

