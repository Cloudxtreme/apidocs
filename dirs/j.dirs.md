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

Utility class to configure and store all relevant directory paths

#### def addProtectedDir(path,name="main") 

#### def amInGitConfigRepo() 

return parent path where .git is or None when not found

#### def checkInProtectedDir(path) 

#### def createGitConfigRepo(path) 

#### def getHrdDir(system=False) 

#### def getPathOfRunningFunction(function) 

#### def init(reinit=False) 

Initializes all the configured directories if needed

If a folder attribute is None, set its value to the corresponding
default path.

@returns: Initialization success
@rtype: bool

#### def isGitConfigRepo(path) 

#### def loadProtectedDirs() 

#### def removeProtectedDir(path) 

#### def replaceTxtDirVars(txt,additionalArgs=\{\}) 

replace $base,$vardir,$cfgDir,$bindir,$codedir,$tmpdir,$logdir,$appdir with props of this class

