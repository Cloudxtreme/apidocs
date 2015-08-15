## j.core.osismodel

- /opt/jumpscale7/lib/JumpScale/grid/osismodel/OSIS.py
- Properties
    - dict2object
    - osisInstances

### Methods

    

#### def destroy 
##### arguments

- appname
- actorname = '*'
- modelname = '*'

##### comments

```
destroy all objects & indexes with mentioned names

```

#### def dict2object 
##### arguments

- obj
- data

##### comments

```

```

#### def get 
##### arguments

- appname
- actorname
- modelname
- modelClass
- db
- index = False
- indexer

##### comments

```

```

#### def getNoDB 
##### arguments

- appname
- actorname
- modelname
- modelClass

##### comments

```

```

#### def getRemoteOsisDB 
##### arguments

- appname
- actorname
- modelname
- modelClass

##### comments

```

```

#### def inputNormalizeList 
##### arguments

- param

##### comments

```
comma separated string becomes list
list gets checked, if all int then returnformat=1
list gets checked, if all str, then returnformat=2
@return (returnformat,list)

```

#### def rebuildindex 
##### arguments

- appname
- actorname = '*'
- modelname = '*'

##### comments

```
destroy all objects & indexes with mentioned names

```

