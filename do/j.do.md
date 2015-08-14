## j.do

- /opt/jumpscale7/lib/JumpScale/InstallTools.py
- Properties
    - TMP
    - BASE
    - debug
    - CODEDIR
    - TYPE

#### def changeDir(path,create=False) 

Changes Current Directory
@param path: string (Directory path to be changed to)

#### def changeLoginPasswdGitRepos(provider,login,passwd) 

walk over all git repo's found in account & change login/passwd

#### def chdir(ddir="") 

if ddir=="" then will go to tmpdir

#### def checkDirOrLinkToDir(fullpath) 

check if path is dir or link to a dir

#### def checkInstalled(cmdname) 

@param cmdname is cmd to check e.g. curl

#### def chmod(path,permissions) 

@param permissions e.g. 0o660 (USE OCTAL !!!)

#### def chown(path,user) 

#### def copyDependencies(path,dest) 

#### def copyFile(source,dest,deletefirst=False,skipIfExists=False) 

#### def copyTree(source, dest, keepsymlinks = False, deletefirst = False, overwriteFiles=True,ignoredir=[".egg-info",".dist-info"],ignorefiles=[".egg-info"],rsync=True,sshkey=None) 

#### def createDir(path) 

#### def delete(path,force=False) 

#### def download(url,to="",overwrite=True,retry=3,timeout=0,login="",passwd="",minspeed=0,multithread=False,curl=False) 

@return path of downloaded file
@param minspeed is kbytes per sec e.g. 50, if less than 50 kbytes during 10 min it will restart the download (curl only)
@param when multithread True then will use aria2 download tool to get multiple threads

#### def downloadExpandTarGz(url,destdir,deleteDestFirst=True,deleteSourceAfter=True) 

#### def downloadJumpScaleCore(dest) 

#### def excepthook(ttype, pythonExceptionObject, tb) 

#### def execute(command , outputStdout=True, outputStderr=True, useShell=True, log=True, cwd=None, timeout=0, errors=[], ok=[], captureout=True, dieOnNonZeroExitCode=True) 

@param errors is array of statements if found then exit as error
return rc,out,err

#### def executeCmds(cmdstr, outputStdout=True, outputStderr=True,useShell = True,log=True,cwd=None,timeout=120,errors=[],ok=[],captureout=True,dieOnNonZeroExitCode=True) 

#### def executeInteractive(command) 

#### def exists(path) 

#### def expandTarGz(path,destdir,deleteDestFirst=True,deleteSourceAfter=False) 

#### def findDependencies(path,deps=\{\}) 

#### def getBaseName(path) 

Return the base name of pathname path.

#### def getDirName(path,lastOnly=False,levelsUp=None) 

Return a directory name from pathname path.
@param path the path to find a directory within
@param lastOnly means only the last part of the path which is a dir (overrides levelsUp to 0)
@param levelsUp means, return the parent dir levelsUp levels up
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=0) would return something
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=1) would return bin
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=10) would raise an error

#### def getFileExtension(path) 

#### def getGitRepoArgs(url="", dest=None, login=None, passwd=None, reset=False) 

Extracts and returns data useful in cloning a Git repository.

Args:
    url (str): the HTTP URL of the Git repository to clone from. ex: 'https://github.com/odoo/odoo.git'
    dest (str): the local filesystem path to clone to
    login (str): authentication login name
    passwd (str): authentication login password
    reset (boolean): if True, any cached clone of the Git repository will be removed

Returns:
    (repository_host, repository_type, repository_account, repository_name, repository_url)

#### def getGitReposListLocal(provider="",account="",name="",errorIfNone=True) 

#### def getParent(path) 

Returns the parent of the path:
/dir1/dir2/file_or_dir -> /dir1/dir2/
/dir1/dir2/            -> /dir1/
@todo why do we have 2 implementations which are almost the same see getParentDirName()

#### def getPythonSiteConfigPath() 

#### def getTimeEpoch() 

Get epoch timestamp (number of seconds passed since January 1, 1970)

#### def getTmpPath(filename) 

#### def getWalker() 

#### def installPackage(path) 

#### def isDir(path, followSoftlink=False) 

Check if the specified Directory path exists
@param path: string
@param followSoftlink: boolean
@rtype: boolean (True if directory exists)

#### def isExecutable(path) 

#### def isFile(path, followSoftlink = False) 

Check if the specified file exists for the given path
@param path: string
@param followSoftlink: boolean
@rtype: boolean (True if file exists for the given path)

#### def isLink(path,checkJunction=False) 

Check if the specified path is a link
@param path: string
@rtype: boolean (True if the specified path is a link)

#### def isUnix() 

#### def isWindows() 

#### def joinPaths(*args) 

#### def list(path) 

#### def listDirsInDir(path,recursive=False,dirNameOnly=False,findDirectorySymlinks=True) 

Retrieves list of directories found in the specified directory
@param path: string represents directory path to search in
@rtype: list

#### def listFilesAndDirsInDir(path, recursive=False, filter=None, minmtime=None, maxmtime=None,depth=None,type="fd",followSymlinks=True,listSymlinks=False) 

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

#### def listFilesInDir(path, recursive=False, filter=None, minmtime=None, maxmtime=None,depth=None, case_sensitivity='os',exclude=[],followSymlinks=True,listSymlinks=False) 

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

#### def loadScript(path) 

#### def log(msg, level=None) 

#### def pullGitRepo(url="",dest=None,login=None,passwd=None,depth=1,ignorelocalchanges=False,reset=False,branch=None,revision=None) 

will clone or update repo
if dest == None then clone underneath: /opt/code/$type/$account/$repo
will ignore changes !!!!!!!!!!!

#### def pushGitRepos(message,name="",update=True,provider="",account="") 

if name specified then will look under code dir if repo with path can be found
if not or more than 1 there will be error
@param provider e.g. git, github

#### def readFile(filename) 

Read a file and get contents of that file
@param filename: string (filename to open for reading )
@rtype: string representing the file contents

#### def readLink(path) 

Works only for unix
Return a string representing the path to which the symbolic link points.

#### def removeLinks(path) 

find all links & remove

#### def removeSymlink(path) 

#### def rewriteGitRepoUrl(url="", login=None, passwd=None) 

Rewrite the url of a git repo with login and passwd if specified

Args:
    url (str): the HTTP URL of the Git repository. ex: 'https://github.com/odoo/odoo'
    login (str): authentication login name
    passwd (str): authentication login password

Returns:
    (repository_host, repository_type, repository_account, repository_name, repository_url)

#### def sendmail(ffrom,to,subject,msg,smtpuser,smtppasswd,smtpserver="smtp.mandrillapp.com",port=587,html="") 

#### def symlink(src,dest,delete=False) 

dest is where the link will be created pointing to src

#### def symlinkFilesInDir(src,dest,delete=True, includeDirs=False) 

#### def touch(path) 

#### def updateGitRepos(provider="",account="",name="",message="") 

#### def writeFile(path,content,strip=True) 

