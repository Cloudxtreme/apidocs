## j.system.platform.lxc

- /opt/jumpscale7/lib/JumpScale/lib/lxc/Lxc.py

### Methods

#### btrfsSubvolCopy 
##### arguments

    - nameFrom
    - NameDest

##### comments

#### btrfsSubvolDelete 
##### arguments

    - name

##### comments

#### btrfsSubvolExists 
##### arguments

    - name

##### comments

#### btrfsSubvolList 
##### arguments

##### comments

#### btrfsSubvolNew 
##### arguments

    - name

##### comments

#### create 
##### arguments

    - name = ''
    - stdout = True
    - base = 'base'
    - start = False
    - nameserver = '8.8.8.8'
    - replace = True

##### comments

@param name if "" then will be an incremental nr

#### destroy 
##### arguments

    - name

##### comments

#### destroyAll 
##### arguments

##### comments

#### execute 
##### arguments

    - command

##### comments

#### exportRsync 
##### arguments

    - name
    - backupname
    - key = 'pub'

##### comments

#### exportTgz 
##### arguments

    - name
    - backupname

##### comments

#### getConfig 
##### arguments

    - name

##### comments

#### getIp 
##### arguments

    - name
    - fail = True

##### comments

#### getPid 
##### arguments

    - name
    - fail = True

##### comments

#### getProcessList 
##### arguments

    - name
    - stdout = True

##### comments

@return [["$name",$pid,$mem,$parent],....,[$mem,$cpu]]
last one is sum of mem & cpu

#### importRsync 
##### arguments

    - backupname
    - name
    - basename = ''
    - key = 'pub'

##### comments

@param basename is the name of a start of a machine locally, will be used as basis and then the source will be synced over it

#### importTgz 
##### arguments

    - backupname
    - name

##### comments

#### list 
##### arguments

##### comments

names of running & stopped machines
@return (running,stopped)

#### networkSet 
##### arguments

    - machinename
    - netname = 'pub0'
    - pubips = []
    - bridge = 'public'
    - gateway

##### comments

#### networkSetPrivateVXLan 
##### arguments

    - name
    - vxlanid
    - ipaddresses

##### comments

#### pushSSHKey 
##### arguments

    - name

##### comments

#### removeRedundantFiles 
##### arguments

    - name

##### comments

#### setHostName 
##### arguments

    - name

##### comments

#### start 
##### arguments

    - name
    - stdout = True
    - test = True

##### comments

#### stop 
##### arguments

    - name

##### comments

