## j.system.platform.lxc

- /opt/jumpscale7/lib/JumpScale/lib/lxc/Lxc.py

### def btrfsSubvolList() (l158)

### def networkSetPrivateVXLan(name, vxlanid, ipaddresses) (l468)

### def btrfsSubvolDelete(name) (l189)

### def getPid(name,fail=True) (l94)

### def removeRedundantFiles(name) (l199)

### def importRsync(backupname,name,basename="",key="pub") (l206)

@param basename is the name of a start of a machine locally, will be used as basis and then the source will be synced over it

### def start(name,stdout=True,test=True) (l393)

### def setHostName(name) (l347)

### def create(name="",stdout=True,base="base",start=False,nameserver="8.8.8.8",replace=True) (l258)

@param name if "" then will be an incremental nr

### def pushSSHKey(name) (l357)

### def btrfsSubvolNew(name) (l171)

### def destroyAll() (l364)

### def btrfsSubvolCopy(nameFrom,NameDest) (l176)

### def destroy(name) (l370)

### def getIp(name,fail=True) (l81)

### def getProcessList(name, stdout=True) (l108)

@return [["$name",$pid,$mem,$parent],....,[$mem,$cpu]]
last one is sum of mem & cpu

### def btrfsSubvolExists(name) (l184)

### def stop(name) (l388)

### def networkSet(machinename,netname="pub0",pubips=[],bridge="public",gateway=None) (l427)

### def execute(command) (l16)

### def importTgz(backupname,name) (l248)

### def list() (l54)

names of running & stopped machines
@return (running,stopped)

### def exportRsync(name,backupname,key="pub") (l139)

### def exportTgz(name,backupname) (l236)

### def getConfig(name) (l85)

