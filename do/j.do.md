## j.do

- /opt/jumpscale7/lib/JumpScale/InstallTools.py
- Properties
    - TMP
    - BASE
    - debug
    - CODEDIR
    - TYPE

### Methods

#### def changeDir 
##### arguments

- path
- create = False

##### comments

Changes Current Directory
@param path: string (Directory path to be changed to)

#### def changeLoginPasswdGitRepos 
##### arguments

- provider
- login
- passwd

##### comments

walk over all git repo's found in account & change login/passwd

#### def chdir 
##### arguments

- ddir = ''

##### comments

if ddir=="" then will go to tmpdir

#### def checkDirOrLinkToDir 
##### arguments

- fullpath

##### comments

check if path is dir or link to a dir

#### def checkInstalled 
##### arguments

- cmdname

##### comments

@param cmdname is cmd to check e.g. curl

#### def chmod 
##### arguments

- path
- permissions

##### comments

@param permissions e.g. 0o660 (USE OCTAL !!!)

#### def chown 
##### arguments

- path
- user

##### comments

#### def copyDependencies 
##### arguments

- path
- dest

##### comments

#### def copyFile 
##### arguments

- source
- dest
- deletefirst = False
- skipIfExists = False

##### comments

#### def copyTree 
##### arguments

- source
- dest
- keepsymlinks = False
- deletefirst = False
- overwriteFiles = True
- ignoredir = ['.egg-info', '.dist-info']
- ignorefiles = ['.egg-info']
- rsync = True
- sshkey

##### comments

#### def createDir 
##### arguments

- path

##### comments

#### def delete 
##### arguments

- path
- force = False

##### comments

#### def download 
##### arguments

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

##### comments

@return path of downloaded file
@param minspeed is kbytes per sec e.g. 50, if less than 50 kbytes during 10 min it will restart the download (curl only)
@param when multithread True then will use aria2 download tool to get multiple threads

#### def downloadExpandTarGz 
##### arguments

- url
- destdir
- deleteDestFirst = True
- deleteSourceAfter = True

##### comments

#### def downloadJumpScaleCore 
##### arguments

- dest

##### comments

#### def excepthook 
##### arguments

- ttype
- pythonExceptionObject
- tb

##### comments

#### def execute 
##### arguments

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

##### comments

@param errors is array of statements if found then exit as error
return rc,out,err

#### def executeCmds 
##### arguments

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

##### comments

#### def executeInteractive 
##### arguments

- command

##### comments

#### def exists 
##### arguments

- path

##### comments

#### def expandTarGz 
##### arguments

- path
- destdir
- deleteDestFirst = True
- deleteSourceAfter = False

##### comments

#### def findDependencies 
##### arguments

- path
- deps = \{\}

##### comments

#### def getBaseName 
##### arguments

- path

##### comments

Return the base name of pathname path.

#### def getDirName 
##### arguments

- path
- lastOnly = False
- levelsUp

##### comments

Return a directory name from pathname path.
@param path the path to find a directory within
@param lastOnly means only the last part of the path which is a dir (overrides levelsUp to 0)
@param levelsUp means, return the parent dir levelsUp levels up
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=0) would return something
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=1) would return bin
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=10) would raise an error

#### def getFileExtension 
##### arguments

- path

##### comments

#### def getGitRepoArgs 
##### arguments

- url = ''
- dest
- login
- passwd
- reset = False

##### comments

Extracts and returns data useful in cloning a Git repository.

Args:
    url (str): the HTTP URL of the Git repository to clone from. ex: 'https://github.com/odoo/odoo.git'
    dest (str): the local filesystem path to clone to
    login (str): authentication login name
    passwd (str): authentication login password
    reset (boolean): if True, any cached clone of the Git repository will be removed

Returns:
    (repository_host, repository_type, repository_account, repository_name, repository_url)

#### def getGitReposListLocal 
##### arguments

- provider = ''
- account = ''
- name = ''
- errorIfNone = True

##### comments

#### def getParent 
##### arguments

- path

##### comments

Returns the parent of the path:
/dir1/dir2/file_or_dir -> /dir1/dir2/
/dir1/dir2/            -> /dir1/
@todo why do we have 2 implementations which are almost the same see getParentDirName()

#### def getPythonSiteConfigPath 
##### arguments

##### comments

#### def getTimeEpoch 
##### arguments

##### comments

Get epoch timestamp (number of seconds passed since January 1, 1970)

#### def getTmpPath 
##### arguments

- filename

##### comments

#### def getWalker 
##### arguments

##### comments

#### def installPackage 
##### arguments

- path

##### comments

#### def isDir 
##### arguments

- path
- followSoftlink = False

##### comments

Check if the specified Directory path exists
@param path: string
@param followSoftlink: boolean
@rtype: boolean (True if directory exists)

#### def isExecutable 
##### arguments

- path

##### comments

#### def isFile 
##### arguments

- path
- followSoftlink = False

##### comments

Check if the specified file exists for the given path
@param path: string
@param followSoftlink: boolean
@rtype: boolean (True if file exists for the given path)

#### def isLink 
##### arguments

- path
- checkJunction = False

##### comments

Check if the specified path is a link
@param path: string
@rtype: boolean (True if the specified path is a link)

#### def isUnix 
##### arguments

##### comments

#### def isWindows 
##### arguments

##### comments

#### def joinPaths 
##### arguments

- *args

##### comments

#### def list 
##### arguments

- path

##### comments

#### def listDirsInDir 
##### arguments

- path
- recursive = False
- dirNameOnly = False
- findDirectorySymlinks = True

##### comments

Retrieves list of directories found in the specified directory
@param path: string represents directory path to search in
@rtype: list

#### def listFilesAndDirsInDir 
##### arguments

- path
- recursive = False
- filter
- minmtime
- maxmtime
- depth
- type = 'fd'
- followSymlinks = True
- listSymlinks = False

##### comments

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

#### def listFilesInDir 
##### arguments

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

##### comments

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

#### def loadScript 
##### arguments

- path

##### comments

#### def log 
##### arguments

- msg
- level

##### comments

#### def pullGitRepo 
##### arguments

- url = ''
- dest
- login
- passwd
- depth = 1
- ignorelocalchanges = False
- reset = False
- branch
- revision

##### comments

will clone or update repo
if dest == None then clone underneath: /opt/code/$type/$account/$repo
will ignore changes !!!!!!!!!!!

#### def pushGitRepos 
##### arguments

- message
- name = ''
- update = True
- provider = ''
- account = ''

##### comments

if name specified then will look under code dir if repo with path can be found
if not or more than 1 there will be error
@param provider e.g. git, github

#### def readFile 
##### arguments

- filename

##### comments

Read a file and get contents of that file
@param filename: string (filename to open for reading )
@rtype: string representing the file contents

#### def readLink 
##### arguments

- path

##### comments

Works only for unix
Return a string representing the path to which the symbolic link points.

#### def removeLinks 
##### arguments

- path

##### comments

find all links & remove

#### def removeSymlink 
##### arguments

- path

##### comments

#### def rewriteGitRepoUrl 
##### arguments

- url = ''
- login
- passwd

##### comments

Rewrite the url of a git repo with login and passwd if specified

Args:
    url (str): the HTTP URL of the Git repository. ex: 'https://github.com/odoo/odoo'
    login (str): authentication login name
    passwd (str): authentication login password

Returns:
    (repository_host, repository_type, repository_account, repository_name, repository_url)

#### def sendmail 
##### arguments

- ffrom
- to
- subject
- msg
- smtpuser
- smtppasswd
- smtpserver = 'smtp.mandrillapp.com'
- port = 587
- html = ''

##### comments

#### def symlink 
##### arguments

- src
- dest
- delete = False

##### comments

dest is where the link will be created pointing to src

#### def symlinkFilesInDir 
##### arguments

- src
- dest
- delete = True
- includeDirs = False

##### comments

#### def touch 
##### arguments

- path

##### comments

#### def updateGitRepos 
##### arguments

- provider = ''
- account = ''
- name = ''
- message = ''

##### comments

#### def writeFile 
##### arguments

- path
- content
- strip = True

##### comments

