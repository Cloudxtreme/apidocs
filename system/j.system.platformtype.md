## j.system.platformtype

- /opt/jumpscale7/lib/JumpScale/core/PlatformTypes.py
- Properties
    - myplatform
    - platformParents

### Methods

#### addPlatform 
##### arguments

    - name
    - parent

##### comments

#### checkMatch 
##### arguments

    - match

##### comments

match is in form of linux64,darwin
if any of the items e.g. darwin is in getMyRelevantPlatforms then return True

#### dieIfNotPlatform 
##### arguments

    - platform

##### comments

#### getChildren 
##### arguments

    - name

##### comments

#### getMyRelevantPlatforms 
##### arguments

##### comments

#### getParents 
##### arguments

    - name

##### comments

#### getPlatforms 
##### arguments

##### comments

#### has_parent 
##### arguments

    - name

##### comments

#### isGeneric 
##### arguments

##### comments

Checks whether the platform is generic (they all should)

#### isHyperV 
##### arguments

##### comments

Check whether the system supports HyperV

#### isLinux 
##### arguments

##### comments

Checks whether the platform is Linux-based

#### isUnix 
##### arguments

##### comments

Checks whether the platform is Unix-based

#### isVirtualBox 
##### arguments

##### comments

Check whether the system supports VirtualBox

#### isWindows 
##### arguments

##### comments

Checks whether the platform is Windows-based

#### isXen 
##### arguments

##### comments

Checks whether Xen support is enabled

