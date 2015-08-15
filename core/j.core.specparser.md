## j.core.specparser

- /opt/jumpscale7/lib/JumpScale/baselib/specparser/SpecParser.py
- Properties
    - actornames
    - roles
    - modelnames
    - app_actornames
    - childspecs
    - appnames
    - specs

### Methods

#### def addSpec 
##### arguments

- spec

##### comments

#### def findSpec 
##### arguments

- query = ''
- appname = ''
- actorname = ''
- specname = ''
- type = ''
- findFromSpec
- findOnlyOne = True

##### comments

do not specify query with one of the other filter criteria
@param query is in dot notation e.g. $appname.$actorname.$modelname ... the items in front are optional

#### def getActorSpec 
##### arguments

- app
- name
- raiseError = True

##### comments

#### def getChildModelSpec 
##### arguments

- app
- actorname
- name
- die = True

##### comments

#### def getEnumerationSpec 
##### arguments

- app
- actorname
- name
- die = True

##### comments

#### def getModelNames 
##### arguments

- appname
- actorname

##### comments

#### def getModelSpec 
##### arguments

- app
- actorname
- name
- die = True

##### comments

#### def getSpecFromTypeStr 
##### arguments

- appname
- actorname
- typestr

##### comments

@param typestr e.g list(machine.status)
@return $returntype,$spec  $returntype=list,dict,object,enum (list & dict can be of primitive types or objects (NOT enums))

#### def init 
##### arguments

##### comments

#### def parseSpecs 
##### arguments

- specpath
- appname
- actorname

##### comments

@param specpath if empty will look for path specs in current dir

#### def removeSpecsForActor 
##### arguments

- appname
- actorname

##### comments

#### def resetMemNonSystem 
##### arguments

##### comments

