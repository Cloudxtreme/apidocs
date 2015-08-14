## j.core.osismodel

- /opt/jumpscale7/lib/JumpScale/grid/osismodel/OSIS.py
- Properties
    - dict2object
    - osisInstances

    

### def rebuildindex(appname, actorname="*", modelname="*") (l59)

destroy all objects & indexes with mentioned names

### def getRemoteOsisDB(appname, actorname, modelname, modelClass=None) (l28)

### def get(appname, actorname, modelname, modelClass=None, db=None, index=False, indexer=None) (l14)

### def dict2JSModelobject(obj,data) (l123)

### def getNoDB(appname, actorname, modelname, modelClass=None) (l21)

### def destroy(appname, actorname="*", modelname="*") (l49)

destroy all objects & indexes with mentioned names

### def inputNormalizeList(param) (l76)

comma separated string becomes list
list gets checked, if all int then returnformat=1
list gets checked, if all str, then returnformat=2
@return (returnformat,list)

