## j.tools.docker

- /opt/jumpscale7/lib/JumpScale/lib/docker/Docker.py
- Properties
    - client

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
#### def commit 
##### arguments

- name
- imagename
#### def copy 
##### arguments

- name
- src
- dest
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
#### def destroyall 
##### arguments

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
#### def exportTgz 
##### arguments

- name
- backupname
#### def getImages 
##### arguments

#### def getInfo 
##### arguments

- name
#### def getIp 
##### arguments

- name
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
#### def getSSH 
##### arguments

- name
- stdout = False
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
#### def inspect 
##### arguments

- name
#### def installJumpscale 
##### arguments

- name
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
#### def pushSSHKey 
##### arguments

- name
#### def removeImages 
##### arguments

- tag = '<none>:<none>'
#### def removeRedundantFiles 
##### arguments

- name
#### def restart 
##### arguments

- name
#### def run 
##### arguments

- name
- cmd
#### def setHostName 
##### arguments

- name
#### def stop 
##### arguments

- name
#### def uploadFile 
##### arguments

- name
- source
- dest

##### comments

```
put a file located at source on the host to dest into the container

```

