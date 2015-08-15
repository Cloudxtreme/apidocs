## j.system.platform.ubuntu

- /opt/jumpscale7/lib/JumpScale/baselib/platforms/ubuntu/Ubuntu.py
- Properties
    - installedPackageNames

### Methods

#### def addSourceUri 
##### arguments

- url
#### def addUser2Group 
##### arguments

- group
- user
#### def changeSourceUri 
##### arguments

- newuri
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

#### def createGroup 
##### arguments

- groupname
#### def createUser 
##### arguments

- name
- passwd
- home
- creategroup = True
- deletefirst = False
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
#### def existsUser 
##### arguments

- name
#### def find1packageInstalled 
##### arguments

- packagename
#### def findPackagesInstalled 
##### arguments

- packagename
#### def findPackagesRepo 
##### arguments

- packagename
#### def generateLocalSSHKeyPair 
##### arguments

- passphrase = ''
- type = 'rsa'
- overwrite = False
- path = '/root/.ssh/id_rsa'
#### def getPackage 
##### arguments

- name
#### def getPackageNamesInstalled 
##### arguments

#### def getPackageNamesRepo 
##### arguments

#### def getVersion 
##### arguments

##### comments

```
returns codename,descr,id,release
known ids" raring, linuxmint

```

#### def initApt 
##### arguments

#### def install 
##### arguments

- packagename
#### def installDebFile 
##### arguments

- path
- installDeps = True
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

#### def remove 
##### arguments

- packagename
#### def restartService 
##### arguments

- servicename
#### def serviceDisableStartAtBoot 
##### arguments

- servicename
#### def serviceEnableStartAtBoot 
##### arguments

- servicename
#### def serviceInstall 
##### arguments

- servicename
- daemonpath
- args = ''
- respawn = True
- pwd
- env
- reload = True
#### def serviceUninstall 
##### arguments

- servicename
#### def startService 
##### arguments

- servicename
#### def statusService 
##### arguments

- servicename
#### def stopService 
##### arguments

- servicename
#### def updatePackageMetadata 
##### arguments

- force = True
#### def upgradePackages 
##### arguments

- force = True
#### def whoami 
##### arguments

