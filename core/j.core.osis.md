## j.core.osis

- /opt/jumpscale7/lib/JumpScale/grid/osis/OSISFactory.py
- Properties
    - osisModels
    - nodeguids
    - namespacesInited

    

    #### def decrypt(val,json=False) 
    #### def encrypt(obj) 
    #### def generateOsisModelDefaults(namespace,specpath="") 
    #### def getLocal(path="", overwriteHRD=False, overwriteImplementation=False, namespacename=None) 
    
    create local instance starting from path
    #### def getModelTemplate() 
    #### def getOSISBaseObjectComplexType() 
    #### def getOsisBaseObjectClass() 
    #### def getOsisImplementationParentClass(namespacename) 
    
    return parent class for osis implementation (is the implementation from which each namespace & category inherits)
    #### def getOsisModelClass(namespace,category,specpath="") 
    
    returns class generated from spec file or from model.py file
    #### def startDaemon(path="", overwriteHRD=False, overwriteImplementation=False, key="",port=5544,superadminpasswd=None,dbconnections=\{\},hrd=None) 
    
    start deamon
