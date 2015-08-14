## j.tools.docker

- /opt/jumpscale7/lib/JumpScale/lib/docker/Docker.py
- Properties
    - client

#### def btrfsSubvolCopy(nameFrom,NameDest) 

    

#### def btrfsSubvolDelete(name) 

    

#### def btrfsSubvolExists(name) 

    

#### def btrfsSubvolList() 

    

#### def btrfsSubvolNew(name) 

    

#### def commit(name,imagename) 

    

#### def copy(name,src,dest) 

    

#### def create(name="",ports="",vols="",volsro="",stdout=True,base="despiegk/mc",nameserver=["8.8.8.8"],replace=True,cpu=None,mem=0,jumpscale=False,ssh=True,myinit=True) 

    @param ports in format as follows  "22:8022 80:8080"  the first arg e.g. 22 is the port in the container
    @param vols in format as follows "/var/insidemachine:/var/inhost # /var/1:/var/1 # ..."   '#' is separator

#### def destroy(name) 

    

#### def destroyall() 

    

#### def downloadFile(name, source, dest) 

    get a file located at source in the host to dest on the host

#### def execute(name,path) 

    execute file in docker

#### def exportRsync(name,backupname,key="pub") 

    

#### def exportTgz(name,backupname) 

    

#### def getImages() 

    

#### def getInfo(name) 

    

#### def getIp(name) 

    

#### def getProcessList(name, stdout=True) 

    @return [["$name",$pid,$mem,$parent],....,[$mem,$cpu]]
    last one is sum of mem & cpu

#### def getPubPortForInternalPort(name,port) 

    

#### def getSSH(name,stdout=False) 

    

#### def importRsync(backupname,name,basename="",key="pub") 

    @param basename is the name of a start of a machine locally, will be used as basis and then the source will be synced over it

#### def importTgz(backupname,name) 

    

#### def inspect(name) 

    

#### def installJumpscale(name) 

    

#### def list() 

    return list of names

#### def ps() 

    return detailed info

#### def pull(imagename) 

    

#### def pushSSHKey(name) 

    

#### def removeImages(tag="<none><none>") 

    

#### def removeRedundantFiles(name) 

    

#### def restart(name) 

    

#### def run(name,cmd) 

    

#### def setHostName(name) 

    

#### def stop(name) 

    

#### def uploadFile(name, source, dest) 

    put a file located at source on the host to dest into the container

