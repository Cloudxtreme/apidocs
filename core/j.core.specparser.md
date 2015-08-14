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

    #### def addSpec(spec) 
    #### def findSpec(query="",appname="",actorname="",specname="",type="",findFromSpec=None,findOnlyOne=True) 
    
    do not specify query with one of the other filter criteria
    @param query is in dot notation e.g. $appname.$actorname.$modelname ... the items in front are optional
    #### def getActorSpec(app,name,raiseError=True) 
    #### def getChildModelSpec(app,actorname,name,die=True) 
    #### def getEnumerationSpec(app,actorname,name,die=True) 
    #### def getModelNames(appname,actorname) 
    #### def getModelSpec(app,actorname,name,die=True) 
    #### def getSpecFromTypeStr(appname,actorname,typestr) 
    
    @param typestr e.g list(machine.status)
    @return $returntype,$spec  $returntype=list,dict,object,enum (list & dict can be of primitive types or objects (NOT enums))
    #### def init() 
    #### def parseSpecs(specpath,appname,actorname) 
    
    @param specpath if empty will look for path specs in current dir
    #### def removeSpecsForActor(appname,actorname) 
    #### def resetMemNonSystem() 
