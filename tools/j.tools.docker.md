## j.tools.docker

- /opt/jumpscale7/lib/JumpScale/lib/docker/Docker.py
- Properties
    - client

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

#### def commit 
##### arguments

- name
- imagename

##### comments

```

```

#### def copy 
##### arguments

- name
- src
- dest

##### comments

```

```

#### def create 
##### arguments

- name = ''
- ports = ''
- vols = ''
- volsro = ''
- stdout = True
- base = 'despiegk/mc'
- nameserver = ['8.8.8.8']
- replace = True
- cpu
- mem = 0
- jumpscale = False
- ssh = True
- myinit = True

##### comments

```
@param ports in format as follows  "22:8022 80:8080"  the first arg e.g. 22 is the port in the container
@param vols in format as follows "/var/insidemachine:/var/inhost # /var/1:/var/1 # ..."   '#' is separator

```

#### def destroy 
##### arguments

- name

##### comments

```

```

#### def destroyall 
##### arguments

##### comments

```

```

#### def downloadFile 
##### arguments

- name
- source
- dest

##### comments

```
get a file located at source in the host to dest on the host

```

#### def execute 
##### arguments

- name
- path

##### comments

```
execute file in docker

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

#### def getImages 
##### arguments

##### comments

```

```

#### def getInfo 
##### arguments

- name

##### comments

```

```

#### def getIp 
##### arguments

- name

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

#### def getPubPortForInternalPort 
##### arguments

- name
- port

##### comments

```

```

#### def getSSH 
##### arguments

- name
- stdout = False

##### comments

```

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

#### def inspect 
##### arguments

- name

##### comments

```

```

#### def installJumpscale 
##### arguments

- name

##### comments

```

```

#### def list 
##### arguments

##### comments

```
return list of names

```

#### def ps 
##### arguments

##### comments

```
return detailed info

```

#### def pull 
##### arguments

- imagename

##### comments

```

```

#### def pushSSHKey 
##### arguments

- name

##### comments

```

```

#### def removeImages 
##### arguments

- tag = '<none>:<none>'

##### comments

```

```

#### def removeRedundantFiles 
##### arguments

- name

##### comments

```

```

#### def restart 
##### arguments

- name

##### comments

```

```

#### def run 
##### arguments

- name
- cmd

##### comments

```

```

#### def setHostName 
##### arguments

- name

##### comments

```

```

#### def stop 
##### arguments

- name

##### comments

```

```

#### def uploadFile 
##### arguments

- name
- source
- dest

##### comments

```
put a file located at source on the host to dest into the container

```

