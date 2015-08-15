## j.tools.inifile

- /opt/jumpscale7/lib/JumpScale/baselib/inifile/IniFile.py

### Methods

#### def new 
##### arguments

- filename

##### comments

Create a new INI file

@param filename: Filename of INI file
@type filename: string

@raises RuntimeError: When the provided filename exists

@returns: New INI file object
@rtype: jumpscale.inifile.IniFile.IniFile

#### def open 
##### arguments

- filename
- createIfNonExisting = True

##### comments

Open an existing INI file

@param filename: Filename of INI file
@type filename: string

@raises RuntimeError: When the provided filename doesn't exist

@returns: Opened INI file object
@rtype: jumpscale.inifile.IniFile.IniFile

