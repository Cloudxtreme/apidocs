## j.do

- /opt/jumpscale7/lib/JumpScale/InstallTools.py
- Properties
    - TMP
    - BASE
    - debug
    - CODEDIR
    - TYPE

### def isDir(path, followSoftlink=False) (l296)

Check if the specified Directory path exists
@param path: string
@param followSoftlink: boolean
@rtype: boolean (True if directory exists)

### def checkDirOrLinkToDir(fullpath) (l458)

check if path is dir or link to a dir

### def exists(path) (l370)

### def joinPaths(*args) (l163)

### def getBaseName(path) (l448)

Return the base name of pathname path.

### def chmod(path,permissions) (l735)

@param permissions e.g. 0o660 (USE OCTAL !!!)

### def getPythonSiteConfigPath() (l1088)

### def download(url,to="",overwrite=True,retry=3,timeout=0,login="",passwd="",minspeed=0,multithread=False,curl=False) (l767)

@return path of downloaded file
@param minspeed is kbytes per sec e.g. 50, if less than 50 kbytes during 10 min it will restart the download (curl only)
@param when multithread True then will use aria2 download tool to get multiple threads

### def removeLinks(path) (l515)

find all links & remove

### def listFilesAndDirsInDir(path, recursive=False, filter=None, minmtime=None, maxmtime=None,depth=None,type="fd",followSymlinks=True,listSymlinks=False) (l596)

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

### def downloadJumpScaleCore(dest) (l1083)

### def excepthook(ttype, pythonExceptionObject, tb) (l83)

### def changeDir(path,create=False) (l281)

Changes Current Directory
@param path: string (Directory path to be changed to)

### def removeSymlink(path) (l436)

### def isLink(path,checkJunction=False) (l329)

Check if the specified path is a link
@param path: string
@rtype: boolean (True if the specified path is a link)

### def executeInteractive(command) (l1033)

### def writeFile(path,content,strip=True) (l116)

### def log(msg, level=None) (l100)

### def isUnix() (l852)

### def getGitReposListLocal(provider="",account="",name="",errorIfNone=True) (l1258)

### def sendmail(ffrom,to,subject,msg,smtpuser,smtppasswd,smtpserver="smtp.mandrillapp.com",port=587,html="") (l877)

### def getDirName(path,lastOnly=False,levelsUp=None) (l470)

Return a directory name from pathname path.
@param path the path to find a directory within
@param lastOnly means only the last part of the path which is a dir (overrides levelsUp to 0)
@param levelsUp means, return the parent dir levelsUp levels up
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=0) would return something
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=1) would return bin
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=10) would raise an error

### def readFile(filename) (l104)

Read a file and get contents of that file
@param filename: string (filename to open for reading )
@rtype: string representing the file contents

### def rewriteGitRepoUrl(url="", login=None, passwd=None) (l1103)

Rewrite the url of a git repo with login and passwd if specified

Args:
    url (str): the HTTP URL of the Git repository. ex: 'https://github.com/odoo/odoo'
    login (str): authentication login name
    passwd (str): authentication login password

Returns:
    (repository_host, repository_type, repository_account, repository_name, repository_url)

### def expandTarGz(path,destdir,deleteDestFirst=True,deleteSourceAfter=False) (l1043)

### def findDependencies(path,deps={}) (l373)

### def installPackage(path) (l1367)

### def getTimeEpoch() (l1097)

Get epoch timestamp (number of seconds passed since January 1, 1970)

### def downloadExpandTarGz(url,destdir,deleteDestFirst=True,deleteSourceAfter=True) (l1037)

### def changeLoginPasswdGitRepos(provider,login,passwd) (l1308)

walk over all git repo's found in account & change login/passwd

### def createDir(path) (l275)

### def getGitRepoArgs(url="", dest=None, login=None, passwd=None, reset=False) (l1151)

Extracts and returns data useful in cloning a Git repository.

Args:
    url (str): the HTTP URL of the Git repository to clone from. ex: 'https://github.com/odoo/odoo.git'
    dest (str): the local filesystem path to clone to
    login (str): authentication login name
    passwd (str): authentication login password
    reset (boolean): if True, any cached clone of the Git repository will be removed

Returns:
    (repository_host, repository_type, repository_account, repository_name, repository_url)

### def isExecutable(path) (l311)

### def pullGitRepo(url="",dest=None,login=None,passwd=None,depth=1,ignorelocalchanges=False,reset=False,branch=None,revision=None) (l1196)

will clone or update repo
if dest == None then clone underneath: /opt/code/$type/$account/$repo
will ignore changes !!!!!!!!!!!

### def touch(path) (l113)

### def pushGitRepos(message,name="",update=True,provider="",account="") (l1277)

if name specified then will look under code dir if repo with path can be found
if not or more than 1 there will be error
@param provider e.g. git, github

### def copyDependencies(path,dest) (l389)

### def updateGitRepos(provider="",account="",name="",message="") (l1297)

### def symlinkFilesInDir(src,dest,delete=True, includeDirs=False) (l425)

### def symlink(src,dest,delete=False) (l396)

dest is where the link will be created pointing to src

### def getTmpPath(filename) (l1080)

### def getWalker() (l1338)

### def loadScript(path) (l1342)

### def isWindows() (l857)

### def getParent(path) (l689)

Returns the parent of the path:
/dir1/dir2/file_or_dir -> /dir1/dir2/
/dir1/dir2/            -> /dir1/
@todo why do we have 2 implementations which are almost the same see getParentDirName()

### def checkInstalled(cmdname) (l1248)

@param cmdname is cmd to check e.g. curl

### def copyFile(source,dest,deletefirst=False,skipIfExists=False) (l259)

### def execute(command , outputStdout=True, outputStderr=True, useShell=True, log=True, cwd=None, timeout=0, errors=[], ok=[], captureout=True, dieOnNonZeroExitCode=True) (l902)

@param errors is array of statements if found then exit as error
return rc,out,err

### def chdir(ddir="") (l757)

if ddir=="" then will go to tmpdir

### def executeCmds(cmdstr, outputStdout=True, outputStderr=True,useShell = True,log=True,cwd=None,timeout=120,errors=[],ok=[],captureout=True,dieOnNonZeroExitCode=True) (l862)

### def getFileExtension(path) (l704)

### def list(path) (l358)

### def chown(path,user) (l712)

### def listDirsInDir(path,recursive=False,dirNameOnly=False,findDirectorySymlinks=True) (l541)

Retrieves list of directories found in the specified directory
@param path: string represents directory path to search in
@rtype: list

### def readLink(path) (l498)

Works only for unix
Return a string representing the path to which the symbolic link points.

### def copyTree(source, dest, keepsymlinks = False, deletefirst = False, overwriteFiles=True,ignoredir=[".egg-info",".dist-info"],ignorefiles=[".egg-info"],rsync=True,sshkey=None) (l166)

### def listFilesInDir(path, recursive=False, filter=None, minmtime=None, maxmtime=None,depth=None, case_sensitivity='os',exclude=[],followSymlinks=True,listSymlinks=False) (l570)

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

### def isFile(path, followSoftlink = False) (l314)

Check if the specified file exists for the given path
@param path: string
@param followSoftlink: boolean
@rtype: boolean (True if file exists for the given path)

### def delete(path,force=False) (l140)

