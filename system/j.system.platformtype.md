## j.system.platformtype

- /opt/jumpscale7/lib/JumpScale/core/PlatformTypes.py
- Properties
    - myplatform
    - platformParents

### def getMyRelevantPlatforms() (l52)

### def isVirtualBox() (l189)

Check whether the system supports VirtualBox

### def isHyperV() (l197)

Check whether the system supports HyperV

### def isUnix() (l169)

Checks whether the platform is Unix-based

### def checkMatch(match) (l55)

match is in form of linux64,darwin
if any of the items e.g. darwin is in getMyRelevantPlatforms then return True

### def isLinux() (l177)

Checks whether the platform is Linux-based

### def isGeneric() (l181)

Checks whether the platform is generic (they all should)

### def dieIfNotPlatform(platform) (l165)

### def getPlatforms() (l68)

### def getChildren(name) (l79)

### def has_parent(name) (l160)

### def isXen() (l185)

Checks whether Xen support is enabled

### def addPlatform(name,parent) (l82)

### def getParents(name) (l71)

### def isWindows() (l173)

Checks whether the platform is Windows-based

