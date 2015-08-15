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

#### def amInGitConfigRepo 

##### arguments

##### comments

```
return parent path where .git is or None when not found

```

#### def checkInProtectedDir 

##### arguments

- path

#### def createGitConfigRepo 

##### arguments

- path

#### def getHrdDir 

##### arguments

- system = False

#### def getPathOfRunningFunction 

##### arguments

- function

#### def init 

##### arguments

- reinit = False

##### comments

```
Initializes all the configured directories if needed

If a folder attribute is None, set its value to the corresponding
default path.

@returns: Initialization success
@rtype: bool

```

#### def isGitConfigRepo 

##### arguments

- path

#### def loadProtectedDirs 

##### arguments

#### def removeProtectedDir 

##### arguments

- path

#### def replaceTxtDirVars 

##### arguments

- txt
- additionalArgs = \{\}

##### comments

```
replace $base,$vardir,$cfgDir,$bindir,$codedir,$tmpdir,$logdir,$appdir with
    props of this class

```

