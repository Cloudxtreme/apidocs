## j.tools.objectinspector

- /opt/jumpscale7/lib/JumpScale/baselib/objectinspector/ObjectInspector.py
- Properties
    - errors
    - dest
    - apiFileLocation
    - base
    - visited
    - classDocs

### Methods

functionality to inspect objectr structure and generate apifile

#### generateDocs 
##### arguments

    - dest
    - ignore = []

##### comments

#### importAllLibs 
##### arguments

    - ignore = []
    - base = '/opt/jumpscale7/lib/JumpScale/'

##### comments

#### inspect 
##### arguments

    - objectLocationPath = 'j'
    - recursive = True
    - parent
    - obj

##### comments

walk over objects in memory and create code completion api in jumpscale cfgDir under codecompletionapi
@param object is start object
@param objectLocationPath is full location name in object tree e.g. j.system.fs , no need to fill in

#### raiseError 
##### arguments

    - errormsg

##### comments

#### writeDocs 
##### arguments

    - path

##### comments

