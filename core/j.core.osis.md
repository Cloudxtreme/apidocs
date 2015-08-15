## j.core.osis

- /opt/jumpscale7/lib/JumpScale/grid/osis/OSISFactory.py
- Properties
    - osisModels
    - nodeguids
    - namespacesInited

    

#### decrypt 
- arguments
    - val
    - json = False
- comments
    

#### encrypt 
- arguments
    - obj
- comments
    

#### generateOsisModelDefaults 
- arguments
    - namespace
    - specpath = ''
- comments
    

#### getLocal 
- arguments
    - path = ''
    - overwriteHRD = False
    - overwriteImplementation = False
    - namespacename
- comments
    create local instance starting from path

#### getModelTemplate 
- arguments
- comments
    

#### getOSISBaseObjectComplexType 
- arguments
- comments
    

#### getOsisBaseObjectClass 
- arguments
- comments
    

#### getOsisImplementationParentClass 
- arguments
    - namespacename
- comments
    return parent class for osis implementation (is the implementation from which each namespace & category inherits)

#### getOsisModelClass 
- arguments
    - namespace
    - category
    - specpath = ''
- comments
    returns class generated from spec file or from model.py file

#### startDaemon 
- arguments
    - path = ''
    - overwriteHRD = False
    - overwriteImplementation = False
    - key = ''
    - port = 5544
    - superadminpasswd
    - dbconnections = \{\}
    - hrd
- comments
    start deamon

