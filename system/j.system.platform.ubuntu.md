## j.system.platform.ubuntu

- /opt/jumpscale7/lib/JumpScale/baselib/platforms/ubuntu/Ubuntu.py
- Properties
    - installedPackageNames

### Methods

#### addSourceUri 
##### arguments

    - url

##### comments

#### addUser2Group 
##### arguments

    - group
    - user

##### comments

#### changeSourceUri 
##### arguments

    - newuri

##### comments

#### check 
##### arguments

    - die = True

##### comments

check if ubuntu or mint (which is based on ubuntu)

#### checkInstall 
##### arguments

    - packagenames
    - cmdname

##### comments

@param packagenames is name or array of names of ubuntu package to install e.g. curl
@param cmdname is cmd to check e.g. curl

#### checkroot 
##### arguments

##### comments

#### createGroup 
##### arguments

    - groupname

##### comments

#### createUser 
##### arguments

    - name
    - passwd
    - home
    - creategroup = True
    - deletefirst = False

##### comments

#### downloadInstallDebPkg 
##### arguments

    - url
    - removeDownloaded = False
    - minspeed = 20

##### comments

will download to tmp if not there yet
will then install

#### existsGroup 
##### arguments

    - name

##### comments

#### existsUser 
##### arguments

    - name

##### comments

#### find1packageInstalled 
##### arguments

    - packagename

##### comments

#### findPackagesInstalled 
##### arguments

    - packagename

##### comments

#### findPackagesRepo 
##### arguments

    - packagename

##### comments

#### generateLocalSSHKeyPair 
##### arguments

    - passphrase = ''
    - type = 'rsa'
    - overwrite = False
    - path = '/root/.ssh/id_rsa'

##### comments

#### getPackage 
##### arguments

    - name

##### comments

#### getPackageNamesInstalled 
##### arguments

##### comments

#### getPackageNamesRepo 
##### arguments

##### comments

#### getVersion 
##### arguments

##### comments

returns codename,descr,id,release
known ids" raring, linuxmint

#### initApt 
##### arguments

##### comments

#### install 
##### arguments

    - packagename

##### comments

#### installDebFile 
##### arguments

    - path
    - installDeps = True

##### comments

#### installVersion 
##### arguments

    - packageName
    - version

##### comments

Installs a specific version of an ubuntu package.

@param packageName: name of the package
@type packageName: str

@param version: version of the package
@type version: str

#### listFilesPkg 
##### arguments

    - pkgname
    - regex = ''

##### comments

list files of dpkg
if regex used only output the ones who are matching regex

#### listSources 
##### arguments

##### comments

#### remove 
##### arguments

    - packagename

##### comments

#### restartService 
##### arguments

    - servicename

##### comments

#### serviceDisableStartAtBoot 
##### arguments

    - servicename

##### comments

#### serviceEnableStartAtBoot 
##### arguments

    - servicename

##### comments

#### serviceInstall 
##### arguments

    - servicename
    - daemonpath
    - args = ''
    - respawn = True
    - pwd
    - env
    - reload = True

##### comments

#### serviceUninstall 
##### arguments

    - servicename

##### comments

#### startService 
##### arguments

    - servicename

##### comments

#### statusService 
##### arguments

    - servicename

##### comments

#### stopService 
##### arguments

    - servicename

##### comments

#### updatePackageMetadata 
##### arguments

    - force = True

##### comments

#### upgradePackages 
##### arguments

    - force = True

##### comments

#### whoami 
##### arguments

##### comments

