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

#### addSpec 
- arguments
    - spec
- comments
    

#### findSpec 
- arguments
    - query = ''
    - appname = ''
    - actorname = ''
    - specname = ''
    - type = ''
    - findFromSpec
    - findOnlyOne = True
- comments
    do not specify query with one of the other filter criteria
    @param query is in dot notation e.g. $appname.$actorname.$modelname ... the items in front are optional

#### getActorSpec 
- arguments
    - app
    - name
    - raiseError = True
- comments
    

#### getChildModelSpec 
- arguments
    - app
    - actorname
    - name
    - die = True
- comments
    

#### getEnumerationSpec 
- arguments
    - app
    - actorname
    - name
    - die = True
- comments
    

#### getModelNames 
- arguments
    - appname
    - actorname
- comments
    

#### getModelSpec 
- arguments
    - app
    - actorname
    - name
    - die = True
- comments
    

#### getSpecFromTypeStr 
- arguments
    - appname
    - actorname
    - typestr
- comments
    @param typestr e.g list(machine.status)
    @return $returntype,$spec  $returntype=list,dict,object,enum (list & dict can be of primitive types or objects (NOT enums))

#### init 
- arguments
- comments
    

#### parseSpecs 
- arguments
    - specpath
    - appname
    - actorname
- comments
    @param specpath if empty will look for path specs in current dir

#### removeSpecsForActor 
- arguments
    - appname
    - actorname
- comments
    

#### resetMemNonSystem 
- arguments
- comments
    

