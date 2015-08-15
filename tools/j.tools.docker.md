## j.tools.docker

- /opt/jumpscale7/lib/JumpScale/lib/docker/Docker.py
- Properties
    - client

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

#### commit 
##### arguments

    - name
    - imagename

##### comments

#### copy 
##### arguments

    - name
    - src
    - dest

##### comments

#### create 
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

@param ports in format as follows  "22:8022 80:8080"  the first arg e.g. 22 is the port in the container
@param vols in format as follows "/var/insidemachine:/var/inhost # /var/1:/var/1 # ..."   '#' is separator

#### destroy 
##### arguments

    - name

##### comments

#### destroyall 
##### arguments

##### comments

#### downloadFile 
##### arguments

    - name
    - source
    - dest

##### comments

get a file located at source in the host to dest on the host

#### execute 
##### arguments

    - name
    - path

##### comments

execute file in docker

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

#### getImages 
##### arguments

##### comments

#### getInfo 
##### arguments

    - name

##### comments

#### getIp 
##### arguments

    - name

##### comments

#### getProcessList 
##### arguments

    - name
    - stdout = True

##### comments

@return [["$name",$pid,$mem,$parent],....,[$mem,$cpu]]
last one is sum of mem & cpu

#### getPubPortForInternalPort 
##### arguments

    - name
    - port

##### comments

#### getSSH 
##### arguments

    - name
    - stdout = False

##### comments

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

#### inspect 
##### arguments

    - name

##### comments

#### installJumpscale 
##### arguments

    - name

##### comments

#### list 
##### arguments

##### comments

return list of names

#### ps 
##### arguments

##### comments

return detailed info

#### pull 
##### arguments

    - imagename

##### comments

#### pushSSHKey 
##### arguments

    - name

##### comments

#### removeImages 
##### arguments

    - tag = '<none>:<none>'

##### comments

#### removeRedundantFiles 
##### arguments

    - name

##### comments

#### restart 
##### arguments

    - name

##### comments

#### run 
##### arguments

    - name
    - cmd

##### comments

#### setHostName 
##### arguments

    - name

##### comments

#### stop 
##### arguments

    - name

##### comments

#### uploadFile 
##### arguments

    - name
    - source
    - dest

##### comments

put a file located at source on the host to dest into the container

