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

### def parseSpecs(specpath,appname,actorname) (l796)

@param specpath if empty will look for path specs in current dir

### def resetMemNonSystem() (l782)

### def getActorSpec(app,name,raiseError=True) (l575)

### def findSpec(query="",appname="",actorname="",specname="",type="",findFromSpec=None,findOnlyOne=True) (l660)

do not specify query with one of the other filter criteria
@param query is in dot notation e.g. $appname.$actorname.$modelname ... the items in front are optional

### def init() (l762)

### def getChildModelSpec(app,actorname,name,die=True) (l598)

### def getModelSpec(app,actorname,name,die=True) (l585)

### def getSpecFromTypeStr(appname,actorname,typestr) (l812)

@param typestr e.g list(machine.status)
@return $returntype,$spec  $returntype=list,dict,object,enum (list & dict can be of primitive types or objects (NOT enums))

### def removeSpecsForActor(appname,actorname) (l765)

### def addSpec(spec) (l617)

### def getModelNames(appname,actorname) (l610)

### def getEnumerationSpec(app,actorname,name,die=True) (l564)

