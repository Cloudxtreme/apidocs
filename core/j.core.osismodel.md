## j.core.osismodel

- /opt/jumpscale7/lib/JumpScale/grid/osismodel/OSIS.py
- Properties
    - dict2object
    - osisInstances

    

#### def destroy(appname, actorname="*", modelname="*") 

destroy all objects & indexes with mentioned names

#### def dict2JSModelobject(obj,data) 

#### def get(appname, actorname, modelname, modelClass=None, db=None, index=False, indexer=None) 

#### def getNoDB(appname, actorname, modelname, modelClass=None) 

#### def getRemoteOsisDB(appname, actorname, modelname, modelClass=None) 

#### def inputNormalizeList(param) 

comma separated string becomes list
list gets checked, if all int then returnformat=1
list gets checked, if all str, then returnformat=2
@return (returnformat,list)

#### def rebuildindex(appname, actorname="*", modelname="*") 

destroy all objects & indexes with mentioned names

