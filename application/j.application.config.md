## j.application.config

- /opt/jumpscale7/lib/JumpScale/baselib/hrd/HRDTree.py
- Properties
    - keepformat
    - name
    - items
    - changed
    - hrds
    - path
    - commentblock
    - prefixWithName

### Methods

#### def add2tree 
##### arguments

- path
- recursive = True

##### comments

#### def add2treeFromContent 
##### arguments

- content

##### comments

#### def applyOnContent 
##### arguments

- content
- additionalArgs = OrderedDict()

##### comments

look for $(name) and replace with hrd value

#### def applyOnDir 
##### arguments

- path
- filter
- minmtime
- maxmtime
- depth
- changeFileName = True
- changeContent = True
- additionalArgs = OrderedDict()

##### comments

look for $(name) and replace with hrd value

#### def applyOnFile 
##### arguments

- path
- additionalArgs = OrderedDict()

##### comments

look for $(name) and replace with hrd value

#### def checkValidity 
##### arguments

- template
- hrddata = OrderedDict()

##### comments

@param template is example hrd content block, which will be used to check against, 
if params not found will be added to existing hrd

#### def delete 
##### arguments

- key

##### comments

#### def exists 
##### arguments

- key

##### comments

#### def get 
##### arguments

- key
- default

##### comments

#### def getBool 
##### arguments

- key
- default

##### comments

#### def getDict 
##### arguments

- key

##### comments

#### def getDictFromPrefix 
##### arguments

- prefix

##### comments

returns values from prefix return as list

#### def getFloat 
##### arguments

- key

##### comments

#### def getHRDAsDict 
##### arguments

##### comments

#### def getHrd 
##### arguments

- key

##### comments

#### def getInt 
##### arguments

- key
- default

##### comments

#### def getList 
##### arguments

- key
- default

##### comments

#### def getListFromPrefix 
##### arguments

- prefix

##### comments

returns values from prefix return as list

#### def getListFromPrefixEachItemDict 
##### arguments

- prefix
- musthave = []
- defaults = OrderedDict()
- aredict = OrderedDict()
- arelist = []
- areint = []
- arebool = []

##### comments

returns values from prefix return as list
each value represents a dict
@param musthave means for each item which is dict, we need to have following keys
@param specifies the defaults
@param aredicts & arelist specifies which types

#### def getStr 
##### arguments

- key
- default

##### comments

#### def listAdd 
##### arguments

- key
- item

##### comments

#### def pop 
##### arguments

- key

##### comments

#### def prefix 
##### arguments

- key
- depth = 0

##### comments

@param depth means prefix level to return

#### def prefixexists 
##### arguments

- key

##### comments

#### def processall 
##### arguments

##### comments

#### def set 
##### arguments

- key
- val
- persistent = True

##### comments

