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

    #### def generateDocs(dest,ignore=[]) 
    #### def importAllLibs(ignore=[],base="/opt/jumpscale7/lib/JumpScale/") 
    #### def inspect(objectLocationPath="j",recursive=True,parent=None,obj=None) 
    
    walk over objects in memory and create code completion api in jumpscale cfgDir under codecompletionapi
    @param object is start object
    @param objectLocationPath is full location name in object tree e.g. j.system.fs , no need to fill in
    #### def raiseError(errormsg) 
    #### def writeDocs(path) 
