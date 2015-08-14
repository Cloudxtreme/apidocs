## j.system.platform.ubuntu

- /opt/jumpscale7/lib/JumpScale/baselib/platforms/ubuntu/Ubuntu.py
- Properties
    - installedPackageNames

### def find1packageInstalled(packagename) (l327)

### def getPackage(name) (l301)

### def upgradePackages(force=True) (l282)

### def existsGroup(name) (l67)

### def restartService(servicename) (l259)

### def installDebFile(path, installDeps=True) (l174)

### def updatePackageMetadata(force=True) (l276)

### def check(die=True) (l30)

check if ubuntu or mint (which is based on ubuntu)

### def installVersion(packageName, version) (l150)

Installs a specific version of an ubuntu package.

@param packageName: name of the package
@type packageName: str

@param version: version of the package
@type version: str

### def stopService(servicename) (l254)

### def addSourceUri(url) (l346)

### def statusService(servicename) (l262)

### def listFilesPkg(pkgname,regex="") (l197)

list files of dpkg
if regex used only output the ones who are matching regex

### def generateLocalSSHKeyPair(passphrase='', type="rsa", overwrite=False, path="/root/.ssh/id_rsa") (l360)

### def checkroot() (l356)

### def existsUser(name) (l60)

### def serviceEnableStartAtBoot(servicename) (l273)

### def createGroup(groupname) (l110)

### def serviceUninstall(servicename) (l243)

### def addUser2Group(group, user) (l117)

### def startService(servicename) (l247)

### def getPackageNamesInstalled() (l292)

### def serviceDisableStartAtBoot(servicename) (l270)

### def checkInstall(packagenames, cmdname) (l124)

@param packagenames is name or array of names of ubuntu package to install e.g. curl
@param cmdname is cmd to check e.g. curl

### def findPackagesRepo(packagename) (l304)

### def createUser(name,passwd,home=None,creategroup=True,deletefirst=False) (l74)

### def changeSourceUri(newuri) (l340)

### def downloadInstallDebPkg(url,removeDownloaded=False,minspeed=20) (l186)

will download to tmp if not there yet
will then install

### def getVersion() (l50)

returns codename,descr,id,release
known ids" raring, linuxmint

### def getPackageNamesRepo() (l289)

### def serviceInstall(servicename, daemonpath, args='', respawn=True, pwd=None,env=None,reload=True) (l223)

### def remove(packagename) (l210)

### def findPackagesInstalled(packagename) (l315)

### def install(packagename) (l144)

### def initApt() (l10)

### def whoami() (l352)

### def listSources() (l336)

