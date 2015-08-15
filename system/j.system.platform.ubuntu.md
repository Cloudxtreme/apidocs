## j.system.platform.ubuntu

- /opt/jumpscale7/lib/JumpScale/baselib/platforms/ubuntu/Ubuntu.py
- Properties
    - installedPackageNames

### Methods

#### def addSourceUri 
##### arguments

- url

##### comments

```

```

#### def addUser2Group 
##### arguments

- group
- user

##### comments

```

```

#### def changeSourceUri 
##### arguments

- newuri

##### comments

```

```

#### def check 
##### arguments

- die = True

##### comments

```
check if ubuntu or mint (which is based on ubuntu)

```

#### def checkInstall 
##### arguments

- packagenames
- cmdname

##### comments

```
@param packagenames is name or array of names of ubuntu package to install e.g. curl
@param cmdname is cmd to check e.g. curl

```

#### def checkroot 
##### arguments

##### comments

```

```

#### def createGroup 
##### arguments

- groupname

##### comments

```

```

#### def createUser 
##### arguments

- name
- passwd
- home
- creategroup = True
- deletefirst = False

##### comments

```

```

#### def downloadInstallDebPkg 
##### arguments

- url
- removeDownloaded = False
- minspeed = 20

##### comments

```
will download to tmp if not there yet
will then install

```

#### def existsGroup 
##### arguments

- name

##### comments

```

```

#### def existsUser 
##### arguments

- name

##### comments

```

```

#### def find1packageInstalled 
##### arguments

- packagename

##### comments

```

```

#### def findPackagesInstalled 
##### arguments

- packagename

##### comments

```

```

#### def findPackagesRepo 
##### arguments

- packagename

##### comments

```

```

#### def generateLocalSSHKeyPair 
##### arguments

- passphrase = ''
- type = 'rsa'
- overwrite = False
- path = '/root/.ssh/id_rsa'

##### comments

```

```

#### def getPackage 
##### arguments

- name

##### comments

```

```

#### def getPackageNamesInstalled 
##### arguments

##### comments

```

```

#### def getPackageNamesRepo 
##### arguments

##### comments

```

```

#### def getVersion 
##### arguments

##### comments

```
returns codename,descr,id,release
known ids" raring, linuxmint

```

#### def initApt 
##### arguments

##### comments

```

```

#### def install 
##### arguments

- packagename

##### comments

```

```

#### def installDebFile 
##### arguments

- path
- installDeps = True

##### comments

```

```

#### def installVersion 
##### arguments

- packageName
- version

##### comments

```
Installs a specific version of an ubuntu package.

@param packageName: name of the package
@type packageName: str

@param version: version of the package
@type version: str

```

#### def listFilesPkg 
##### arguments

- pkgname
- regex = ''

##### comments

```
list files of dpkg
if regex used only output the ones who are matching regex

```

#### def listSources 
##### arguments

##### comments

```

```

#### def remove 
##### arguments

- packagename

##### comments

```

```

#### def restartService 
##### arguments

- servicename

##### comments

```

```

#### def serviceDisableStartAtBoot 
##### arguments

- servicename

##### comments

```

```

#### def serviceEnableStartAtBoot 
##### arguments

- servicename

##### comments

```

```

#### def serviceInstall 
##### arguments

- servicename
- daemonpath
- args = ''
- respawn = True
- pwd
- env
- reload = True

##### comments

```

```

#### def serviceUninstall 
##### arguments

- servicename

##### comments

```

```

#### def startService 
##### arguments

- servicename

##### comments

```

```

#### def statusService 
##### arguments

- servicename

##### comments

```

```

#### def stopService 
##### arguments

- servicename

##### comments

```

```

#### def updatePackageMetadata 
##### arguments

- force = True

##### comments

```

```

#### def upgradePackages 
##### arguments

- force = True

##### comments

```

```

#### def whoami 
##### arguments

##### comments

```

```

