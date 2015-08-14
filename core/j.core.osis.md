## j.core.osis

- /opt/jumpscale7/lib/JumpScale/grid/osis/OSISFactory.py
- Properties
    - osisModels
    - nodeguids
    - namespacesInited

    

### def getOsisImplementationParentClass(namespacename) (l204)

return parent class for osis implementation (is the implementation from which each namespace & category inherits)

### def getOSISBaseObjectComplexType() (l201)

### def getModelTemplate() (l283)

### def generateOsisModelDefaults(namespace,specpath="") (l271)

### def getOsisBaseObjectClass() (l198)

### def decrypt(val,json=False) (l159)

### def encrypt(obj) (l144)

### def getOsisModelClass(namespace,category,specpath="") (l288)

returns class generated from spec file or from model.py file

### def startDaemon(path="", overwriteHRD=False, overwriteImplementation=False, key="",port=5544,superadminpasswd=None,dbconnections={},hrd=None) (l176)

start deamon

### def getLocal(path="", overwriteHRD=False, overwriteImplementation=False, namespacename=None) (l168)

create local instance starting from path

