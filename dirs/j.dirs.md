## j.dirs

- /opt/jumpscale7/lib/JumpScale/core/Dirs.py
- Properties
    - cfgDir
    - pidDir
    - codeDir
    - binDir
    - appDir
    - baseDir
    - libDir
    - gitConfigDir
    - logDir
    - varDir
    - libExtDir
    - jsLibDir
    - tmpDir

### Methods

Utility class to configure and store all relevant directory paths

#### def addProtectedDir 
##### arguments

- path
- name = 'main'

##### comments

#### def amInGitConfigRepo 
##### arguments

##### comments

return parent path where .git is or None when not found

#### def checkInProtectedDir 
##### arguments

- path

##### comments

#### def createGitConfigRepo 
##### arguments

- path

##### comments

#### def getHrdDir 
##### arguments

- system = False

##### comments

#### def getPathOfRunningFunction 
##### arguments

- function

##### comments

#### def init 
##### arguments

- reinit = False

##### comments

Initializes all the configured directories if needed

If a folder attribute is None, set its value to the corresponding
default path.

@returns: Initialization success
@rtype: bool

#### def isGitConfigRepo 
##### arguments

- path

##### comments

#### def loadProtectedDirs 
##### arguments

##### comments

#### def removeProtectedDir 
##### arguments

- path

##### comments

#### def replaceTxtDirVars 
##### arguments

- txt
- additionalArgs = \{\}

##### comments

replace $base,$vardir,$cfgDir,$bindir,$codedir,$tmpdir,$logdir,$appdir with props of this class

