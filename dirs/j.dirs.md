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

### def checkInProtectedDir(path) (l240)

### def getHrdDir(system=False) (l118)

### def isGitConfigRepo(path) (l261)

### def loadProtectedDirs() (l188)

### def removeProtectedDir(path) (l219)

### def addProtectedDir(path,name="main") (l207)

### def init(reinit=False) (l143)

Initializes all the configured directories if needed

If a folder attribute is None, set its value to the corresponding
default path.

@returns: Initialization success
@rtype: bool

### def getPathOfRunningFunction(function) (l185)

### def createGitConfigRepo(path) (l273)

### def amInGitConfigRepo() (l266)

return parent path where .git is or None when not found

### def replaceTxtDirVars(txt,additionalArgs=\{\}) (l71)

replace $base,$vardir,$cfgDir,$bindir,$codedir,$tmpdir,$logdir,$appdir with props of this class

