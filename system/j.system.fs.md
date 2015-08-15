## j.system.fs

- /opt/jumpscale7/lib/JumpScale/core/system/fs.py
- Properties
    - loglevel
    - logenable

### Methods

#### def changeDir 
##### arguments

- path

##### comments

```
Changes Current Directory
@param path: string (Directory path to be changed to)

```

#### def changeFileNames 
##### arguments

- toReplace
- replaceWith
- pathToSearchIn
- recursive = True
- filter
- minmtime
- maxmtime

##### comments

```
@param toReplace e.g. \{name\}
@param replace with e.g. "jumpscale"

```

#### def checkDirOrLink 
##### arguments

- fullpath

##### comments

```
check if path is dir or link to a dir

```

#### def checkDirOrLinkToDir 
##### arguments

- fullpath

##### comments

```
check if path is dir or link to a dir

```

#### def checkDirParam 
##### arguments

- path
#### def chmod 
##### arguments

- path
- permissions

##### comments

```
@param permissions e.g. 0o660 (USE OCTAL !!!)

```

#### def chown 
##### arguments

- path
- user
#### def cleanupString 
##### arguments

- string
- replacewith = '_'
- regex = '([^A-Za-z0-9])'

##### comments

```
Remove all non-numeric or alphanumeric characters

```

#### def constructDirPathFromArray 
##### arguments

- array
#### def constructFilePathFromArray 
##### arguments

- array
#### def convertFileDirnamesSpaceToUnderscore 
##### arguments

- rootdir
#### def convertFileDirnamesUnicodeToAscii 
##### arguments

- rootdir
- spacesToUnderscore = False
#### def copyDirTree 
##### arguments

- src
- dst
- keepsymlinks = False
- eraseDestination = False
- skipProtectedDirs = False
- overwriteFiles = True
- applyHrdOnDestPaths

##### comments

```
Recursively copy an entire directory tree rooted at src.
The dst directory may already exist; if not,
it will be created as well as missing parent directories
@param src: string (source of directory tree to be copied)
@param dst: string (path directory to be copied to...should not already exist)
@param keepsymlinks: bool (True keeps symlinks instead of copying the content of the file)
@param eraseDestination: bool (Set to True if you want to erase destination first, be carefull, this can erase directories)
@param overwriteFiles: if True will overwrite files, otherwise will not overwrite when destination exists

```

#### def copyFile 
##### arguments

- fileFrom
- to
- createDirIfNeeded = False
- skipProtectedDirs = False
- overwriteFile = True

##### comments

```
Copy file

Copies the file from C\{fileFrom\} to the file or directory C\{to\}.
If C\{to\} is a directory, a file with the same basename as C\{fileFrom\} is
created (or overwritten) in the directory specified.
Permission bits are copied.

@param fileFrom: Source file path name
@type fileFrom: string
@param to: Destination file or folder path name
@type to: string

```

#### def createDir 
##### arguments

- newdir
- skipProtectedDirs = False

##### comments

```
Create new Directory
@param newdir: string (Directory path/name)
if newdir was only given as a directory name, the new directory will be created on the default path,
if newdir was given as a complete path with the directory name, the new directory will be created in the specified path

```

#### def createEmptyFile 
##### arguments

- filename

##### comments

```
Create an empty file
@param filename: string (file path name to be created)

```

#### def dirEqual 
##### arguments

- path1
- path2
#### def exists 
##### arguments

- path
- followlinks = True

##### comments

```
Check if the specified path exists
@param path: string
@rtype: boolean (True if path refers to an existing path)

```

#### def fileConvertLineEndingCRLF 
##### arguments

- file

##### comments

```
Convert CRLF line-endings in a file to LF-only endings (
 -> 
)

        @param file: File to convert
        @type file: string

```

#### def fileGetContents 
##### arguments

- filename

##### comments

```
Read a file and get contents of that file
@param filename: string (filename to open for reading )
@rtype: string representing the file contents

```

#### def fileGetTextContents 
##### arguments

- filename

##### comments

```
Read a UTF-8 file and get contents of that file. Takes care of the [BOM](http://en.wikipedia.org/wiki/Byte_order_mark)
@param filename: string (filename to open for reading)
@rtype: string representing the file contents

```

#### def fileGetUncommentedContents 
##### arguments

- filename

##### comments

```
Read a file and get uncommented contents of that file
@param filename: string (filename to open for reading )
@rtype: list of lines of uncommented file contents

```

#### def fileSize 
##### arguments

- filename

##### comments

```
Get Filesize of file in bytes
@param filename: the file u want to know the filesize of
@return: int representing file size

```

#### def find 
##### arguments

- startDir
- fileregex

##### comments

```
Search for files or folders matching a given pattern
this is a very weard function, don't use is better to use the list functions
make sure you do changedir to the starting dir first
example: find("*.pyc")
@param fileregex: The regex pattern to match
@type fileregex: string

```

#### def getBaseName 
##### arguments

- path

##### comments

```
Return the base name of pathname path.

```

#### def getDirName 
##### arguments

- path
- lastOnly = False
- levelsUp

##### comments

```
Return a directory name from pathname path.
@param path the path to find a directory within
@param lastOnly means only the last part of the path which is a dir (overrides levelsUp to 0)
@param levelsUp means, return the parent dir levelsUp levels up
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=0) would return something
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=1) would return bin
 e.g. ...getDirName("/opt/qbase/bin/something/test.py", levelsUp=10) would raise an error

```

#### def getFileExtension 
##### arguments

- path
#### def getFolderMD5sum 
##### arguments

- folder
#### def getParent 
##### arguments

- path

##### comments

```
Returns the parent of the path:
/dir1/dir2/file_or_dir -> /dir1/dir2/
/dir1/dir2/            -> /dir1/
@todo why do we have 2 implementations which are almost the same see getParentDirName()

```

#### def getParentDirName 
##### arguments

- path

##### comments

```
returns parent of path (only for dirs)
returns empty string when there is no parent

```

#### def getTempFileName 
##### arguments

- dir
- prefix = ''

##### comments

```
Generates a temp file for the directory specified
@param dir: Directory to generate the temp file
@param prefix: string to start the generated name with
@rtype: string representing the generated temp file path

```

#### def getTmpDirPath 
##### arguments

##### comments

```
create a tmp dir name and makes sure the dir exists

```

#### def getTmpFilePath 
##### arguments

- cygwin = False

##### comments

```
Generate a temp file path
Located in temp dir of qbase
@rtype: string representing the path of the temp file generated

```

#### def getcwd 
##### arguments

##### comments

```
get current working directory
@rtype: string (current working directory path)

```

#### def grep 
##### arguments

- fileregex
- lineregex

##### comments

```
Search for lines matching a given regex in all files matching a regex

@param fileregex: Files to search in
@type fileregex: string
@param lineregex: Regex pattern to search for in each file
@type lineregex: string

```

#### def gunzip 
##### arguments

- sourceFile
- destFile
#### def gzip 
##### arguments

- sourceFile
- destFile
#### def hardlinkFile 
##### arguments

- source
- destin

##### comments

```
Create a hard link pointing to source named destin. Availability: Unix.
@param source: string
@param destin: string
@rtype: concatenation of dirname, and optionally linkname, etc.
with exactly one directory separator (os.sep) inserted between components, unless path2 is empty

```

#### def isAsciiFile 
##### arguments

- filename
- checksize = 4096

##### comments

```
Read the first <checksize> bytes of <filename>.
          Validate that only valid ascii characters (32-126), ,       , 
are
          present in the file

```

#### def isBinaryFile 
##### arguments

- filename
- checksize = 4096
#### def isDir 
##### arguments

- path
- followSoftlink = True

##### comments

```
Check if the specified Directory path exists
@param path: string
@param followSoftlink: boolean
@rtype: boolean (True if directory exists)

```

#### def isEmptyDir 
##### arguments

- path

##### comments

```
Check if the specified directory path is empty
@param path: string
@rtype: boolean (True if directory is empty)

```

#### def isExecutable 
##### arguments

- path
#### def isFile 
##### arguments

- path
- followSoftlink = True

##### comments

```
Check if the specified file exists for the given path
@param path: string
@param followSoftlink: boolean
@rtype: boolean (True if file exists for the given path)

```

#### def isLink 
##### arguments

- path
- checkJunction = False

##### comments

```
Check if the specified path is a link
@param path: string
@rtype: boolean (True if the specified path is a link)

```

#### def isMount 
##### arguments

- path

##### comments

```
Return true if pathname path is a mount point:
A point in a file system where a different file system has been mounted.

```

#### def islocked 
##### arguments

- lockname
- reentry = False

##### comments

```
Check if a system-wide interprocess exclusive lock is set

```

#### def joinPaths 
##### arguments

- *args

##### comments

```
Join one or more path components.
If any component is an absolute path, all previous components are thrown away, and joining continues.
@param path1: string
@param path2: string
@param path3: string
@param .... : string
@rtype: Concatenation of path1, and optionally path2, etc...,
with exactly one directory separator (os.sep) inserted between components, unless path2 is empty.

```

#### def listDirsInDir 
##### arguments

- path
- recursive = False
- dirNameOnly = False
- findDirectorySymlinks = True

##### comments

```
Retrieves list of directories found in the specified directory
@param path: string represents directory path to search in
@rtype: list

```

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

```
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

```

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

```
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

```

#### def listPyScriptsInDir 
##### arguments

- path
- recursive = True
- filter = '*.py'

##### comments

```
Retrieves list of python scripts (with extension .py) in the specified directory
@param path: string represents the directory path to search in
@rtype: list

```

#### def lock 
##### arguments

- lockname
- locktimeout = 60
- reentry = False

##### comments

```
Take a system-wide interprocess exclusive lock. Default timeout is 60 seconds

```

#### def lock_ 
##### arguments

- lockname
- locktimeout = 60
- reentry = False

##### comments

```
Take a system-wide interprocess exclusive lock.

Works similar to j.system.fs.lock but uses return values to denote lock
success instead of raising fatal errors.

This refactoring was mainly done to make the lock implementation easier
to unit-test.

```

#### def log 
##### arguments

- msg
- level = 5
- category = ''
#### def md5sum 
##### arguments

- filename

##### comments

```
Return the hex digest of a file without loading it all into memory
@param filename: string (filename to get the hex digest of it) or list of files
@rtype: md5 of the file

```

#### def move 
##### arguments

- source
- destin

##### comments

```
Main Move function
@param source: string (If the specified source is a File....Calls moveFile function)
(If the specified source is a Directory....Calls moveDir function)

```

#### def moveDir 
##### arguments

- source
- destin

##### comments

```
Move Directory from source to destination
@param source: string (Source path where the directory should be removed from)
@param destin: string (Destination path where the directory should be moved into)

```

#### def moveFile 
##### arguments

- source
- destin

##### comments

```
Move a  File from source path to destination path
@param source: string (Source file path)
@param destination: string (Destination path the file should be moved to )

```

#### def parsePath 
##### arguments

- path
- baseDir = ''
- existCheck = True
- checkIsFile = False

##### comments

```
parse paths of form /root/tmp/33_adoc.doc into the path, priority which is numbers before _ at beginning of path
also returns filename
checks if path can be found, if not will fail
when filename="" then is directory which has been parsed
if basedir specified that part of path will be removed

example:
j.system.fs.parsePath("/opt/qbase3/apps/specs/myspecs/definitions/cloud/datacenter.txt","/opt/qbase3/apps/specs/myspecs/",existCheck=False)
@param path is existing path to a file
@param baseDir, is the absolute part of the path not required
@return list of dirpath,filename,extension,priority
     priority = 0 if not specified

```

#### def pathClean 
##### arguments

- path

##### comments

```
goal is to get a equal representation in / & \ in relation to os.sep

```

#### def pathDirClean 
##### arguments

- path
#### def pathNormalize 
##### arguments

- path
- root = ''

##### comments

```
paths are made absolute & made sure they are in line with os.sep
@param path: path to normalize
@root is std the application you are in, can overrule

```

#### def pathRemoveDirPart 
##### arguments

- path
- toremove
- removeTrailingSlash = False

##### comments

```
goal remove dirparts of a dirpath e,g, a basepath which is not needed
will look for part to remove in full path but only full dirs

```

#### def pathShorten 
##### arguments

- path

##### comments

```
Clean path (change /var/www/../lib to /var/lib). On Windows, if the
path exists, the short path name is returned.

@param path: Path to clean
@type path: string
@return: Cleaned (short) path
@rtype: string

```

#### def pathToUnicode 
##### arguments

- path

##### comments

```
Convert path to unicode. Use the local filesystem encoding. Will return
path unmodified if path already is unicode.

Use this to convert paths you received from the os module to unicode.

@param path: path to convert to unicode
@type path: basestring
@return: unicode path
@rtype: unicode

```

#### def processPathForDoubleDots 
##### arguments

- path

##### comments

```
/root/somepath/.. would become /root
/root/../somepath/ would become /somepath

result will always be with / slashes

```

#### def readObjectFromFile 
##### arguments

- filelocation

##### comments

```
Read a object from a file(file contents in pickle format)
@param filelocation: location of the file
@return: object

```

#### def readlink 
##### arguments

- path

##### comments

```
Works only for unix
Return a string representing the path to which the symbolic link points.

```

#### def remove 
##### arguments

- path

##### comments

```
Remove a File
@param path: string (File path required to be removed

```

#### def removeDir 
##### arguments

- path

##### comments

```
Remove a Directory
@param path: string (Directory path that should be removed)

```

#### def removeDirTree 
##### arguments

- path
- onlyLogWarningOnRemoveError = False

##### comments

```
Recursively delete a directory tree.
@param path: the path to be removed

```

#### def removeIrrelevantFiles 
##### arguments

- path
- followSymlinks = True
#### def removeLinks 
##### arguments

- path

##### comments

```
find all links & remove

```

#### def renameDir 
##### arguments

- dirname
- newname
- overwrite = False

##### comments

```
Rename Directory from dirname to newname
@param dirname: string (Directory original name)
@param newname: string (Directory new name to be changed to)

```

#### def renameFile 
##### arguments

- filePath
- new_name

##### comments

```
OBSOLETE

```

#### def replaceWordsInFiles 
##### arguments

- pathToSearchIn
- templateengine
- recursive = True
- filter
- minmtime
- maxmtime

##### comments

```
apply templateengine to list of found files
@param templateengine =te  #example below
    te=j.codetools.templateengine.new()
    te.add("name",self.a.name)
    te.add("description",self.ayses.description)
    te.add("version",self.ayses.version)

```

#### def statPath 
##### arguments

- path

##### comments

```
Perform a stat() system call on the given path
@rtype: object whose attributes correspond to the members of the stat structure

```

#### def symlink 
##### arguments

- path
- target
- overwriteTarget = False

##### comments

```
Create a symbolic link
@param path: source path desired to create a symbolic link for
@param target: destination path required to create the symbolic link at
@param overwriteTarget: boolean indicating whether target can be overwritten

```

#### def targzCompress 
##### arguments

- sourcepath
- destinationpath
- followlinks = False
- destInTar = ''
- pathRegexIncludes = ['.[a-zA-Z0-9]*']
- pathRegexExcludes = []
- contentRegexIncludes = []
- contentRegexExcludes = []
- depths = []
- extrafiles = []

##### comments

```
@param sourcepath: Source directory .
@param destination: Destination filename.
@param followlinks: do not tar the links, follow the link and add that file or content of directory to the tar
@param pathRegexIncludes: / Excludes  match paths to array of regex expressions (array(strings))
@param contentRegexIncludes: / Excludes match content of files to array of regex expressions (array(strings))
@param depths: array of depth values e.g. only return depth 0 & 1 (would mean first dir depth and then 1 more deep) (array(int))
@param destInTar when not specified the dirs, files under sourcedirpath will be added to root of
          tar.gz with this param can put something in front e.g. /qbase3/ prefix to dest in tgz
@param extrafiles is array of array [[source,destpath],[source,destpath],...]  adds extra files to tar
(TAR-GZ-Archive *.tar.gz)

```

#### def targzUncompress 
##### arguments

- sourceFile
- destinationdir
- removeDestinationdir = True

##### comments

```
compress dirname recursive
@param sourceFile: file to uncompress
@param destinationpath: path of to destiniation dir, sourcefile will end up uncompressed in destination dir

```

#### def touch 
##### arguments

- paths
- overwrite = True

##### comments

```
can be single path or multiple (then list)

```

#### def unlink 
##### arguments

- filename

##### comments

```
Remove the given file if it's a file or a symlink

@param filename: File path to be removed
@type filename: string

```

#### def unlinkFile 
##### arguments

- filename

##### comments

```
Remove the file path (only for files, not for symlinks)
@param filename: File path to be removed

```

#### def unlock 
##### arguments

- lockname

##### comments

```
Unlock system-wide interprocess lock

```

#### def unlock_ 
##### arguments

- lockname

##### comments

```
Unlock system-wide interprocess lock

Works similar to j.system.fs.unlock but uses return values to denote unlock
success instead of raising fatal errors.

This refactoring was mainly done to make the lock implementation easier
to unit-test.

```

#### def validateFilename 
##### arguments

- filename
- platform

##### comments

```
Validate a filename for a given (or current) platform

Check whether a given filename is valid on a given platform, or the
current platform if no platform is specified.

Rules
=====
Generic
-------
Zero-length filenames are not allowed

Unix
----
Filenames can contain any character except 0x00. We also disallow a
forward slash ('/') in filenames.

Filenames can be up to 255 characters long.

Windows
-------
Filenames should not contain any character in the 0x00-0x1F range, '<',
'>', ':', '"', '/', '', '|', '?' or '*'. Names should not end with a
dot ('.') or a space (' ').

Several basenames are not allowed, including CON, PRN, AUX, CLOCK$,
NUL, COM[1-9] and LPT[1-9].

Filenames can be up to 255 characters long.

Information sources
===================
Restrictions are based on information found at these URLs:

 * http://en.wikipedia.org/wiki/Filename
 * http://msdn.microsoft.com/en-us/library/aa365247.aspx
 * http://www.boost.org/doc/libs/1_35_0/libs/filesystem/doc/portability_guide.htm
 * http://blogs.msdn.com/brian_dewey/archive/2004/01/19/60263.aspx

@param filename: Filename to check
@type filename: string
@param platform: Platform to validate against
@type platform: L\{PlatformType\}

@returns: Whether the filename is valid on the given platform
@rtype: bool

```

#### def walk 
##### arguments

- root
- recurse = 0
- pattern = '*'
- return_folders = 0
- return_files = 1
- followSoftlinks = True
- str = False
- depth

##### comments

```
This is to provide ScanDir similar function
It is going to be used wherever some one wants to list all files and subfolders
under one given directly with specific or none matchers

```

#### def walkExtended 
##### arguments

- root
- recurse = 0
- dirPattern = '*'
- filePattern = '*'
- followSoftLinks = True
- dirs = True
- files = True

##### comments

```
Extended Walk version: seperate dir and file pattern
@param  root                : start directory to start the search.
@type   root                : string
@param  recurse             : search also in subdirectories.
@type   recurse             : number
@param  dirPattern          : search pattern to match directory names. Wildcards can be included.
@type   dirPattern          : string
@param  filePattern         : search pattern to match file names. Wildcards can be included.
@type   filePattern         : string
@param  followSoftLinks     : determine if links must be followed.
@type   followSoftLinks     : boolean
@param  dirs                : determine to return dir results.
@type   dirs                : boolean
@param  files               : determine to return file results.
@type   files               : boolean

@return                     : List of files and / or directories that match the search patterns.
@rtype                      : list of strings

General guidelines in the usage of the method be means of some examples come next. For the example in /tmp there is

* a file test.rtt
* and ./folder1/subfolder/subsubfolder/small_test/test.rtt

To find the first test you can use
   j.system.fs.walkExtended('/tmp/', dirPattern="*tmp*", filePattern="*.rtt")
To find only the second one you could use
   j.system.fs.walkExtended('tmp', recurse=0, dirPattern="*small_test*", filePattern="*.rtt", dirs=False)

```

#### def writeFile 
##### arguments

- filename
- contents
- append = False

##### comments

```
Open a file and write file contents, close file afterwards
@param contents: string (file contents to be written)

```

#### def writeObjectToFile 
##### arguments

- filelocation
- obj

##### comments

```
Write a object to a file(pickle format)
@param filelocation: location of the file to which we write
@param obj: object to pickle and write to a file

```

