## j.core.osis

- /opt/jumpscale7/lib/JumpScale/grid/osis/OSISFactory.py
- Properties
    - osisModels
    - nodeguids
    - namespacesInited

### Methods

    

#### def decrypt 

##### arguments

- val
- json = False

#### def encrypt 

##### arguments

- obj

#### def generateOsisModelDefaults 

##### arguments

- namespace
- specpath = ''

#### def getLocal 

##### arguments

- path = ''
- overwriteHRD = False
- overwriteImplementation = False
- namespacename

##### comments

```
create local instance starting from path

```

#### def getModelTemplate 

##### arguments

#### def getOSISBaseObjectComplexType 

##### arguments

#### def getOsisBaseObjectClass 

##### arguments

#### def getOsisImplementationParentClass 

##### arguments

- namespacename

##### comments

```
return parent class for osis implementation (is the implementation from which
    each namespace & category inherits)

```

#### def getOsisModelClass 

##### arguments

- namespace
- category
- specpath = ''

##### comments

```
returns class generated from spec file or from model.py file

```

#### def startDaemon 

##### arguments

- path = ''
- overwriteHRD = False
- overwriteImplementation = False
- key = ''
- port = 5544
- superadminpasswd
- dbconnections = \{\}
- hrd

##### comments

```
start deamon

```

