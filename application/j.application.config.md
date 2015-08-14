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

#### def add2tree(path,recursive=True) 

#### def add2treeFromContent(content) 

#### def applyOnContent(content,additionalArgs=OrderedDict()) 

look for $(name) and replace with hrd value

#### def applyOnDir(path,filter=None, minmtime=None, maxmtime=None, depth=None,changeFileName=True,changeContent=True,additionalArgs=OrderedDict()) 

look for $(name) and replace with hrd value

#### def applyOnFile(path,additionalArgs=OrderedDict()) 

look for $(name) and replace with hrd value

#### def checkValidity(template,hrddata=OrderedDict()) 

@param template is example hrd content block, which will be used to check against, 
if params not found will be added to existing hrd

#### def delete(key) 

#### def exists(key) 

#### def get(key,default=None,) 

#### def getBool(key,default=None) 

#### def getDict(key) 

#### def getDictFromPrefix(prefix) 

returns values from prefix return as list

#### def getFloat(key) 

#### def getHRDAsDict() 

#### def getHrd(key) 

#### def getInt(key,default=None) 

#### def getList(key,default=None) 

#### def getListFromPrefix(prefix) 

returns values from prefix return as list

#### def getListFromPrefixEachItemDict(prefix,musthave=[],defaults=OrderedDict(),aredict=OrderedDict(),arelist=[],areint=[],arebool=[]) 

returns values from prefix return as list
each value represents a dict
@param musthave means for each item which is dict, we need to have following keys
@param specifies the defaults
@param aredicts & arelist specifies which types

#### def getStr(key,default=None) 

#### def listAdd(key,item) 

#### def pop(key) 

#### def prefix(key,depth=0) 

@param depth means prefix level to return

#### def prefixexists(key) 

#### def processall() 

#### def set(key,val,persistent=True) 

