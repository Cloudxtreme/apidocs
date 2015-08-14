## j.system.platform.lxc

- /opt/jumpscale7/lib/JumpScale/lib/lxc/Lxc.py

    #### def btrfsSubvolCopy(nameFrom,NameDest) 
    #### def btrfsSubvolDelete(name) 
    #### def btrfsSubvolExists(name) 
    #### def btrfsSubvolList() 
    #### def btrfsSubvolNew(name) 
    #### def create(name="",stdout=True,base="base",start=False,nameserver="8.8.8.8",replace=True) 
    
    @param name if "" then will be an incremental nr
    #### def destroy(name) 
    #### def destroyAll() 
    #### def execute(command) 
    #### def exportRsync(name,backupname,key="pub") 
    #### def exportTgz(name,backupname) 
    #### def getConfig(name) 
    #### def getIp(name,fail=True) 
    #### def getPid(name,fail=True) 
    #### def getProcessList(name, stdout=True) 
    
    @return [["$name",$pid,$mem,$parent],....,[$mem,$cpu]]
    last one is sum of mem & cpu
    #### def importRsync(backupname,name,basename="",key="pub") 
    
    @param basename is the name of a start of a machine locally, will be used as basis and then the source will be synced over it
    #### def importTgz(backupname,name) 
    #### def list() 
    
    names of running & stopped machines
    @return (running,stopped)
    #### def networkSet(machinename,netname="pub0",pubips=[],bridge="public",gateway=None) 
    #### def networkSetPrivateVXLan(name, vxlanid, ipaddresses) 
    #### def pushSSHKey(name) 
    #### def removeRedundantFiles(name) 
    #### def setHostName(name) 
    #### def start(name,stdout=True,test=True) 
    #### def stop(name) 
