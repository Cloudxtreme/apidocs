## j.do

- /opt/jumpscale7/lib/JumpScale/InstallTools.py
- Properties
    - TMP
    - BASE
    - debug
    - CODEDIR
    - TYPE

#### changeDir 
- arguments
    - path
    - create = False
- comments
    Changes Current Directory
    @param path: string (Directory path to be changed to)

#### changeLoginPasswdGitRepos 
- arguments
    - provider
    - login
    - passwd
- comments
    walk over all git repo's found in account & change login/passwd

#### chdir 
- arguments
    - ddir = ''
- comments
    if ddir=="" then will go to tmpdir

#### checkDirOrLinkToDir 
- arguments
    - fullpath
- comments
    check if path is dir or link to a dir

#### checkInstalled 
- arguments
    - cmdname
- comments
    @param cmdname is cmd to check e.g. curl

#### chmod 
- arguments
    - path
    - permissions
- comments
    @param permissions e.g. 0o660 (USE OCTAL !!!)

#### chown 
- arguments
    - path
    - user
- comments
    

#### copyDependencies 
- arguments
    - path
    - dest
- comments
    

#### copyFile 
- arguments
    - source
    - dest
    - deletefirst = False
    - skipIfExists = False
- comments
    

#### copyTree 
- arguments
    - source
    - dest
    - keepsymlinks = False
    - deletefirst = False
    - overwriteFiles = True
    - ignoredir = ['.egg-info', '.dist-info']
    - ignorefiles = ['.egg-info']
    - rsync = True
    - sshkey
- comments
    

#### createDir 
- arguments
    - path
- comments
    

#### delete 
- arguments
    - path
    - force = False
- comments
    

#### download 
- arguments
    - url
    - to = ''
    - overwrite = True
    - retry = 3
    - timeout = 0
    - login = ''
    - passwd = ''
    - minspeed = 0
    - multithread = False
    - curl = False
- comments
    @return path of downloaded file
    @param minspeed is kbytes per sec e.g. 50, if less than 50 kbytes during 10 min it will restart the download (curl only)
    @param when multithread True then will use aria2 download tool to get multiple threads

#### downloadExpandTarGz 
- arguments
    - url
    - destdir
    - deleteDestFirst = True
    - deleteSourceAfter = True
- comments
    

#### downloadJumpScaleCore 
- arguments
    - dest
- comments
    

#### excepthook 
- arguments
    - ttype
    - pythonExceptionObject
    - tb
- comments
    

#### execute 
- arguments
    - command
    - outputStdout = True
    - outputStderr = True
    - useShell = True
    - log = True
    - cwd
    - timeout = 0
    - errors = []
    - ok = []
    - captureout = True
    - dieOnNonZeroExitCode = True
- comments
    @param errors is array of statements if found then exit as error
    return rc,out,err

#### executeCmds 
- arguments
    - cmdstr
    - outputStdout = True
    - outputStderr = True
    - useShell = True
    - log = True
    - cwd
    - timeout = 120
    - errors = []
    - ok = []
    - captureout = True
    - dieOnNonZeroExitCode = True
- comments
    

#### executeInteractive 
- arguments
    - command
- comments
    

#### exists 
- arguments
    - path
- comments
    

#### expandTarGz 
- arguments
    - path
    - destdir
    - deleteDestFirst = True
    - deleteSourceAfter = False
- comments
    

#### findDependencies 
- arguments
    - path
    - deps = \{\}
- comments
    

#### getBaseName 
- arguments
    - path
- comments
    Return the base name of pathname path.

#### getDirName 
- arguments
    - path
    - lastOnly = False
    - levelsUp
- comments
    Return a directory name from pathname path.
    @param path the path to find a directory within
    @param lastOnly means only the last part of the path which is a dir (overrides levelsUp to 0)
    @param levelsUp means, return the parent dir levelsUp levels up
     e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=0) would return something
     e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=1) would return bin
     e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=10) would raise an error

#### getFileExtension 
- arguments
    - path
- comments
    

#### getGitRepoArgs 
- arguments
    - url = ''
    - dest
    - login
    - passwd
    - reset = False
- comments
    Extracts and returns data useful in cloning a Git repository.
    
    Args:
        url (str): the HTTP URL of the Git repository to clone from. ex: 'https://github.com/odoo/odoo.git'
        dest (str): the local filesystem path to clone to
        login (str): authentication login name
        passwd (str): authentication login password
        reset (boolean): if True, any cached clone of the Git repository will be removed
    
    Returns:
        (repository_host, repository_type, repository_account, repository_name, repository_url)

#### getGitReposListLocal 
- arguments
    - provider = ''
    - account = ''
    - name = ''
    - errorIfNone = True
- comments
    

#### getParent 
- arguments
    - path
- comments
    Returns the parent of the path:
    /dir1/dir2/file_or_dir -> /dir1/dir2/
    /dir1/dir2/            -> /dir1/
    @todo why do we have 2 implementations which are almost the same see getParentDirName()

#### getPythonSiteConfigPath 
- arguments
- comments
    

#### getTimeEpoch 
- arguments
- comments
    Get epoch timestamp (number of seconds passed since January 1, 1970)

#### getTmpPath 
- arguments
    - filename
- comments
    

#### getWalker 
- arguments
- comments
    

#### installPackage 
- arguments
    - path
- comments
    

#### isDir 
- arguments
    - path
    - followSoftlink = False
- comments
    Check if the specified Directory path exists
    @param path: string
    @param followSoftlink: boolean
    @rtype: boolean (True if directory exists)

#### isExecutable 
- arguments
    - path
- comments
    

#### isFile 
- arguments
    - path
    - followSoftlink = False
- comments
    Check if the specified file exists for the given path
    @param path: string
    @param followSoftlink: boolean
    @rtype: boolean (True if file exists for the given path)

#### isLink 
- arguments
    - path
    - checkJunction = False
- comments
    Check if the specified path is a link
    @param path: string
    @rtype: boolean (True if the specified path is a link)

#### isUnix 
- arguments
- comments
    

#### isWindows 
- arguments
- comments
    

#### joinPaths 
- arguments
    - *args
- comments
    

#### list 
- arguments
    - path
- comments
    

#### listDirsInDir 
- arguments
    - path
    - recursive = False
    - dirNameOnly = False
    - findDirectorySymlinks = True
- comments
    Retrieves list of directories found in the specified directory
    @param path: string represents directory path to search in
    @rtype: list

#### listFilesAndDirsInDir 
- arguments
    - path
    - recursive = False
    - filter
    - minmtime
    - maxmtime
    - depth
    - type = 'fd'
    - followSymlinks = True
    - listSymlinks = False
- comments
    Retrieves list of files found in the specified directory
    @param path:       directory path to search in
    @type  path:       string
    @param recursive:  recursively look in all subdirs
    @type  recursive:  boolean
    @param filter:     unix-style wildcard (e.g. *.py) - this is not a regular expression
    @type  filter:     string
    @param minmtime:   if not None, only return files whose last modification time > minmtime (epoch in seconds)
    @type  minmtime:   integer
    @param maxmtime:   if not None, only return files whose last modification time < maxmtime (epoch in seconds)
    @Param depth: is levels deep wich we need to go
    @type  maxmtime:   integer
    @param type is string with f & d inside (f for when to find files, d for when to find dirs)
    @rtype: list

#### listFilesInDir 
- arguments
    - path
    - recursive = False
    - filter
    - minmtime
    - maxmtime
    - depth
    - case_sensitivity = 'os'
    - exclude = []
    - followSymlinks = True
    - listSymlinks = False
- comments
    Retrieves list of files found in the specified directory
    @param path:       directory path to search in
    @type  path:       string
    @param recursive:  recursively look in all subdirs
    @type  recursive:  boolean
    @param filter:     unix-style wildcard (e.g. *.py) - this is not a regular expression
    @type  filter:     string
    @param minmtime:   if not None, only return files whose last modification time > minmtime (epoch in seconds)
    @type  minmtime:   integer
    @param maxmtime:   if not None, only return files whose last modification time < maxmtime (epoch in seconds)
    @Param depth: is levels deep wich we need to go
    @type  maxmtime:   integer
    @Param exclude: list of std filters if matches then exclude
    @rtype: list

#### loadScript 
- arguments
    - path
- comments
    

#### log 
- arguments
    - msg
    - level
- comments
    

#### pullGitRepo 
- arguments
    - url = ''
    - dest
    - login
    - passwd
    - depth = 1
    - ignorelocalchanges = False
    - reset = False
    - branch
    - revision
- comments
    will clone or update repo
    if dest == None then clone underneath: /opt/code/$type/$account/$repo
    will ignore changes !!!!!!!!!!!

#### pushGitRepos 
- arguments
    - message
    - name = ''
    - update = True
    - provider = ''
    - account = ''
- comments
    if name specified then will look under code dir if repo with path can be found
    if not or more than 1 there will be error
    @param provider e.g. git, github

#### readFile 
- arguments
    - filename
- comments
    Read a file and get contents of that file
    @param filename: string (filename to open for reading )
    @rtype: string representing the file contents

#### readLink 
- arguments
    - path
- comments
    Works only for unix
    Return a string representing the path to which the symbolic link points.

#### removeLinks 
- arguments
    - path
- comments
    find all links & remove

#### removeSymlink 
- arguments
    - path
- comments
    

#### rewriteGitRepoUrl 
- arguments
    - url = ''
    - login
    - passwd
- comments
    Rewrite the url of a git repo with login and passwd if specified
    
    Args:
        url (str): the HTTP URL of the Git repository. ex: 'https://github.com/odoo/odoo'
        login (str): authentication login name
        passwd (str): authentication login password
    
    Returns:
        (repository_host, repository_type, repository_account, repository_name, repository_url)

#### sendmail 
- arguments
    - ffrom
    - to
    - subject
    - msg
    - smtpuser
    - smtppasswd
    - smtpserver = 'smtp.mandrillapp.com'
    - port = 587
    - html = ''
- comments
    

#### symlink 
- arguments
    - src
    - dest
    - delete = False
- comments
    dest is where the link will be created pointing to src

#### symlinkFilesInDir 
- arguments
    - src
    - dest
    - delete = True
    - includeDirs = False
- comments
    

#### touch 
- arguments
    - path
- comments
    

#### updateGitRepos 
- arguments
    - provider = ''
    - account = ''
    - name = ''
    - message = ''
- comments
    

#### writeFile 
- arguments
    - path
    - content
    - strip = True
- comments
    

