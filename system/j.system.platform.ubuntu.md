## j.system.platform.ubuntu

- /opt/jumpscale7/lib/JumpScale/baselib/platforms/ubuntu/Ubuntu.py
- Properties
    - installedPackageNames

#### def addSourceUri(url) 

#### def addUser2Group(group, user) 

#### def changeSourceUri(newuri) 

#### def check(die=True) 

check if ubuntu or mint (which is based on ubuntu)

#### def checkInstall(packagenames, cmdname) 

@param packagenames is name or array of names of ubuntu package to install e.g. curl
@param cmdname is cmd to check e.g. curl

#### def checkroot() 

#### def createGroup(groupname) 

#### def createUser(name,passwd,home=None,creategroup=True,deletefirst=False) 

#### def downloadInstallDebPkg(url,removeDownloaded=False,minspeed=20) 

will download to tmp if not there yet
will then install

#### def existsGroup(name) 

#### def existsUser(name) 

#### def find1packageInstalled(packagename) 

#### def findPackagesInstalled(packagename) 

#### def findPackagesRepo(packagename) 

#### def generateLocalSSHKeyPair(passphrase='', type="rsa", overwrite=False, path="/root/.ssh/id_rsa") 

#### def getPackage(name) 

#### def getPackageNamesInstalled() 

#### def getPackageNamesRepo() 

#### def getVersion() 

returns codename,descr,id,release
known ids" raring, linuxmint

#### def initApt() 

#### def install(packagename) 

#### def installDebFile(path, installDeps=True) 

#### def installVersion(packageName, version) 

Installs a specific version of an ubuntu package.

@param packageName: name of the package
@type packageName: str

@param version: version of the package
@type version: str

#### def listFilesPkg(pkgname,regex="") 

list files of dpkg
if regex used only output the ones who are matching regex

#### def listSources() 

#### def remove(packagename) 

#### def restartService(servicename) 

#### def serviceDisableStartAtBoot(servicename) 

#### def serviceEnableStartAtBoot(servicename) 

#### def serviceInstall(servicename, daemonpath, args='', respawn=True, pwd=None,env=None,reload=True) 

#### def serviceUninstall(servicename) 

#### def startService(servicename) 

#### def statusService(servicename) 

#### def stopService(servicename) 

#### def updatePackageMetadata(force=True) 

#### def upgradePackages(force=True) 

#### def whoami() 

