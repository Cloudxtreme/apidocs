## j.tools.objectinspector

- /opt/jumpscale7/lib/JumpScale/baselib/objectinspector/ObjectInspector.py
- Properties
    - errors
    - dest
    - apiFileLocation
    - base
    - visited
    - classDocs

functionality to inspect objectr structure and generate apifile

### def raiseError(errormsg) (l139)

### def writeDocs(path) (l283)

### def inspect(objectLocationPath="j",recursive=True,parent=None,obj=None) (l175)

walk over objects in memory and create code completion api in jumpscale cfgDir under codecompletionapi
@param object is start object
@param objectLocationPath is full location name in object tree e.g. j.system.fs , no need to fill in

### def generateDocs(dest,ignore=[]) (l148)

### def importAllLibs(ignore=[],base="/opt/jumpscale7/lib/JumpScale/") (l120)

