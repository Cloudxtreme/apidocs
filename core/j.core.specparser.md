<!-- toc -->
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

```
do not specify query with one of the other filter criteria
@param query is in dot notation e.g. $appname.$actorname.$modelname ... the items in front
    are optional

```

#### def getActorSpec 

##### arguments

- app
- name
- raiseError = True

#### def getChildModelSpec 

##### arguments

- app
- actorname
- name
- die = True

#### def getEnumerationSpec 

##### arguments

- app
- actorname
- name
- die = True

#### def getModelNames 

##### arguments

- appname
- actorname

#### def getModelSpec 

##### arguments

- app
- actorname
- name
- die = True

#### def getSpecFromTypeStr 

##### arguments

- appname
- actorname
- typestr

##### comments

```
@param typestr e.g list(machine.status)
@return $returntype,$spec  $returntype=list,dict,object,enum (list & dict can be of
    primitive types or objects (NOT enums))

```

#### def init 

##### arguments

#### def parseSpecs 

##### arguments

- specpath
- appname
- actorname

##### comments

```
@param specpath if empty will look for path specs in current dir

```

#### def removeSpecsForActor 

##### arguments

- appname
- actorname

#### def resetMemNonSystem 

##### arguments

