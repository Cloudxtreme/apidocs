## j.core.osismodel

- /opt/jumpscale7/lib/JumpScale/grid/osismodel/OSIS.py
- Properties
    - dict2object
    - osisInstances

    

#### destroy 
- arguments
    - appname
    - actorname = '*'
    - modelname = '*'
- comments
    destroy all objects & indexes with mentioned names

#### dict2object 
- arguments
    - obj
    - data
- comments
    

#### get 
- arguments
    - appname
    - actorname
    - modelname
    - modelClass
    - db
    - index = False
    - indexer
- comments
    

#### getNoDB 
- arguments
    - appname
    - actorname
    - modelname
    - modelClass
- comments
    

#### getRemoteOsisDB 
- arguments
    - appname
    - actorname
    - modelname
    - modelClass
- comments
    

#### inputNormalizeList 
- arguments
    - param
- comments
    comma separated string becomes list
    list gets checked, if all int then returnformat=1
    list gets checked, if all str, then returnformat=2
    @return (returnformat,list)

#### rebuildindex 
- arguments
    - appname
    - actorname = '*'
    - modelname = '*'
- comments
    destroy all objects & indexes with mentioned names

