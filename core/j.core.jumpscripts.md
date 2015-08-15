<!-- toc -->
## j.core.jumpscripts

- /opt/jumpscale7/lib/JumpScale/grid/jumpscripts/JumpscriptFactory.py
- Properties
    - basedir

### Methods

    

#### def getArchivedJumpscripts 

##### arguments

- bz2_compressed = True
- types = ('processmanager', 'jumpscripts')

##### comments

```
Returns the available jumpscripts in TAR format that is optionally compressed using bzip2.

Args:
    bz2_compressed (boolean): If True then the returned TAR is bzip2-compressed
    types (sequence of str): A sequence of the types of jumpscripts to be packed in the
    returned archive.
        possible values in the sequence are 'processmanager', 'jumpscripts', and
    'luajumpscripts'.

```

#### def getJSClass 

##### arguments

#### def introspectLuaJumpscript 

##### arguments

- path

##### comments

```
Introspects for a Lua Jumpscript at the given path and returns a LuaJumpscript object with
    the results.

Args:
    path (str): the absolute path to the jumpscript file.

Raises:
    IOError if the file at the path could not be opened.

```

#### def loadFromAC 

##### arguments

- acl

#### def loadFromTar 

##### arguments

- tarcontent
- type

