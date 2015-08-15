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

#### addProtectedDir 
##### arguments

    - path
    - name = 'main'

##### comments

#### amInGitConfigRepo 
##### arguments

##### comments

return parent path where .git is or None when not found

#### checkInProtectedDir 
##### arguments

    - path

##### comments

#### createGitConfigRepo 
##### arguments

    - path

##### comments

#### getHrdDir 
##### arguments

    - system = False

##### comments

#### getPathOfRunningFunction 
##### arguments

    - function

##### comments

#### init 
##### arguments

    - reinit = False

##### comments

Initializes all the configured directories if needed

If a folder attribute is None, set its value to the corresponding
default path.

@returns: Initialization success
@rtype: bool

#### isGitConfigRepo 
##### arguments

    - path

##### comments

#### loadProtectedDirs 
##### arguments

##### comments

#### removeProtectedDir 
##### arguments

    - path

##### comments

#### replaceTxtDirVars 
##### arguments

    - txt
    - additionalArgs = \{\}

##### comments

replace $base,$vardir,$cfgDir,$bindir,$codedir,$tmpdir,$logdir,$appdir with props of this class

