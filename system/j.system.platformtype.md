## j.system.platformtype

- /opt/jumpscale7/lib/JumpScale/core/PlatformTypes.py
- Properties
    - myplatform
    - platformParents

### Methods

#### def addPlatform 
##### arguments

- name
- parent

##### comments

```

```

#### def checkMatch 
##### arguments

- match

##### comments

```
match is in form of linux64,darwin
if any of the items e.g. darwin is in getMyRelevantPlatforms then return True

```

#### def dieIfNotPlatform 
##### arguments

- platform

##### comments

```

```

#### def getChildren 
##### arguments

- name

##### comments

```

```

#### def getMyRelevantPlatforms 
##### arguments

##### comments

```

```

#### def getParents 
##### arguments

- name

##### comments

```

```

#### def getPlatforms 
##### arguments

##### comments

```

```

#### def has_parent 
##### arguments

- name

##### comments

```

```

#### def isGeneric 
##### arguments

##### comments

```
Checks whether the platform is generic (they all should)

```

#### def isHyperV 
##### arguments

##### comments

```
Check whether the system supports HyperV

```

#### def isLinux 
##### arguments

##### comments

```
Checks whether the platform is Linux-based

```

#### def isUnix 
##### arguments

##### comments

```
Checks whether the platform is Unix-based

```

#### def isVirtualBox 
##### arguments

##### comments

```
Check whether the system supports VirtualBox

```

#### def isWindows 
##### arguments

##### comments

```
Checks whether the platform is Windows-based

```

#### def isXen 
##### arguments

##### comments

```
Checks whether Xen support is enabled

```

