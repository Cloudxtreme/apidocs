## j.tools.inifile

- /opt/jumpscale7/lib/JumpScale/baselib/inifile/IniFile.py

### @staticmethod (l31)

Create a new INI file

@param filename: Filename of INI file
@type filename: string

@raises RuntimeError: When the provided filename exists

@returns: New INI file object
@rtype: jumpscale.inifile.IniFile.IniFile

### @staticmethod (l12)

Open an existing INI file

@param filename: Filename of INI file
@type filename: string

@raises RuntimeError: When the provided filename doesn't exist

@returns: Opened INI file object
@rtype: jumpscale.inifile.IniFile.IniFile

