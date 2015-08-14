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

### def applyOnContent(content,additionalArgs=OrderedDict()) (l268)

look for $(name) and replace with hrd value

### def set(key,val,persistent=True) (l42)

### def exists(key) (l64)

### def pop(key) (l238)

### def getStr(key,default=None) (l46)

### def getDictFromPrefix(prefix) (l103)

returns values from prefix return as list

### def prefix(key,depth=0) (l7)

@param depth means prefix level to return

### def getHrd(key) (l37)

### def getListFromPrefix(prefix) (l94)

returns values from prefix return as list

### def getDict(key) (l84)

### def add2tree(path,recursive=True) (l29)

### def checkValidity(template,hrddata=OrderedDict()) (l218)

@param template is example hrd content block, which will be used to check against, 
if params not found will be added to existing hrd

### def getListFromPrefixEachItemDict(prefix,musthave=[],defaults=OrderedDict(),aredict=OrderedDict(),arelist=[],areint=[],arebool=[]) (l144)

returns values from prefix return as list
each value represents a dict
@param musthave means for each item which is dict, we need to have following keys
@param specifies the defaults
@param aredicts & arelist specifies which types

### def applyOnDir(path,filter=None, minmtime=None, maxmtime=None, depth=None,changeFileName=True,changeContent=True,additionalArgs=OrderedDict()) (l242)

look for $(name) and replace with hrd value

### def add2treeFromContent(content) (l23)

### def applyOnFile(path,additionalArgs=OrderedDict()) (l258)

look for $(name) and replace with hrd value

### def get(key,default=None,) (l50)

### def getBool(key,default=None) (l30)

### def listAdd(key,item) (l54)

### def getInt(key,default=None) (l40)

### def getHRDAsDict() (l117)

### def getFloat(key) (l60)

### def prefixexists(key) (l22)

### def getList(key,default=None) (l67)

### def processall() (l234)

### def delete(key) (l46)

