## j.system.platformtype

- /opt/jumpscale7/lib/JumpScale/core/PlatformTypes.py
- Properties
    - myplatform
    - platformParents

#### def addPlatform(name,parent) 

#### def checkMatch(match) 

match is in form of linux64,darwin
if any of the items e.g. darwin is in getMyRelevantPlatforms then return True

#### def dieIfNotPlatform(platform) 

#### def getChildren(name) 

#### def getMyRelevantPlatforms() 

#### def getParents(name) 

#### def getPlatforms() 

#### def has_parent(name) 

#### def isGeneric() 

Checks whether the platform is generic (they all should)

#### def isHyperV() 

Check whether the system supports HyperV

#### def isLinux() 

Checks whether the platform is Linux-based

#### def isUnix() 

Checks whether the platform is Unix-based

#### def isVirtualBox() 

Check whether the system supports VirtualBox

#### def isWindows() 

Checks whether the platform is Windows-based

#### def isXen() 

Checks whether Xen support is enabled

