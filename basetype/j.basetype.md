## j.basetype

- /opt/jumpscale7/lib/JumpScale/core/pmtypes/__init__.py
- Properties
    - ipport
    - set
    - string
    - dictionary
    - windowsdirpath
    - float
    - list
    - unixfilepath
    - object
    - filepath
    - duration
    - ipaddressrange
    - boolean
    - windowsfilepath
    - path
    - dirpath
    - integer
    - guid
    - ipaddress
    - unixdirpath
    - enumeration

### Methods

#### def enumeration 
##### arguments

- enumerationtype
- **kwargs

##### comments

Generic descriptor generator for custom enumeration types

You should be aware this is, unlike non-generic basetypes, a function
generating a class instance, not a class.

@param enumerationtype: Type of which values should be instances
@type enumerationtype: Subclass of L\{jumpscale.baseclasses.BaseEnumeration.BaseEnumeration\}
@param kwargs: Kwargs sent to L\{jumpscale.pmtypes.base.BaseType.__init__\}

@returns: An instance of a custom descriptor class
@rtype: L\{jumpscale.pmtypes.base.BaseType.__init__\}

@see: L\{jumpscale.pmtypes.base.BaseType.__init__\}

#### def object 
##### arguments

- type_
- **kwargs

##### comments

Generic descriptor generator for custom object types

You should be aware this is, unlike non-generic basetypes, a function
generating a class instance, not a class.

@param type_: Type of which values should be instances
@type type_: class or type
@param kwargs: Kwargs sent to L\{jumpscale.pmtypes.base.BaseType.__init__\}

@returns: An instance of a custom descriptor class
@rtype: L\{jumpscale.pmtypes.base.BaseType.__init__\}

@see: L\{jumpscale.pmtypes.base.BaseType.__init__\}

