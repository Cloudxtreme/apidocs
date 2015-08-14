## j.tools.docker

- /opt/jumpscale7/lib/JumpScale/lib/docker/Docker.py
- Properties
    - client

### def btrfsSubvolList() (l164)

### def installJumpscale(name) (l417)

### def list() (l81)

return list of names

### def downloadFile(name, source, dest) (l568)

get a file located at source in the host to dest on the host

### def destroyall() (l514)

### def removeRedundantFiles(name) (l210)

### def importRsync(backupname,name,basename="",key="pub") (l218)

@param basename is the name of a start of a machine locally, will be used as basis and then the source will be synced over it

### def ps() (l90)

return detailed info

### def getSSH(name,stdout=False) (l505)

### def getPubPortForInternalPort(name,port) (l449)

### def uploadFile(name, source, dest) (l562)

put a file located at source on the host to dest into the container

### def setHostName(name) (l438)

### def create(name="",ports="",vols="",volsro="",stdout=True,base="despiegk/mc",nameserver=["8.8.8.8"],replace=True,cpu=None,mem=0,jumpscale=False,ssh=True,myinit=True) (l273)

@param ports in format as follows  "22:8022 80:8080"  the first arg e.g. 22 is the port in the container
@param vols in format as follows "/var/insidemachine:/var/inhost # /var/1:/var/1 # ..."   '#' is separator

### def pushSSHKey(name) (l457)

### def btrfsSubvolNew(name) (l178)

### def btrfsSubvolCopy(nameFrom,NameDest) (l184)

### def destroy(name) (l532)

### def getIp(name) (l108)

### def getProcessList(name, stdout=True) (l112)

@return [["$name",$pid,$mem,$parent],....,[$mem,$cpu]]
last one is sum of mem & cpu

### def run(name,cmd) (l28)

### def btrfsSubvolExists(name) (l193)

### def inspect(name) (l96)

### def stop(name) (l543)

### def copy(name,src,dest) (l39)

### def restart(name) (l549)

### def pull(imagename) (l558)

### def execute(name,path) (l32)

execute file in docker

### def getImages() (l428)

### def getInfo(name) (l102)

### def importTgz(backupname,name) (l262)

### def btrfsSubvolDelete(name) (l199)

### def exportRsync(name,backupname,key="pub") (l144)

### def exportTgz(name,backupname) (l249)

### def commit(name,imagename) (l552)

### def removeImages(tag="<none><none>") (l432)

