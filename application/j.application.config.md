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

#### add2tree 
- arguments
    - path
    - recursive = True
- comments
    

#### add2treeFromContent 
- arguments
    - content
- comments
    

#### applyOnContent 
- arguments
    - content
    - additionalArgs = OrderedDict()
- comments
    look for $(name) and replace with hrd value

#### applyOnDir 
- arguments
    - path
    - filter
    - minmtime
    - maxmtime
    - depth
    - changeFileName = True
    - changeContent = True
    - additionalArgs = OrderedDict()
- comments
    look for $(name) and replace with hrd value

#### applyOnFile 
- arguments
    - path
    - additionalArgs = OrderedDict()
- comments
    look for $(name) and replace with hrd value

#### checkValidity 
- arguments
    - template
    - hrddata = OrderedDict()
- comments
    @param template is example hrd content block, which will be used to check against, 
    if params not found will be added to existing hrd

#### delete 
- arguments
    - key
- comments
    

#### exists 
- arguments
    - key
- comments
    

#### get 
- arguments
    - key
    - default
- comments
    

#### getBool 
- arguments
    - key
    - default
- comments
    

#### getDict 
- arguments
    - key
- comments
    

#### getDictFromPrefix 
- arguments
    - prefix
- comments
    returns values from prefix return as list

#### getFloat 
- arguments
    - key
- comments
    

#### getHRDAsDict 
- arguments
- comments
    

#### getHrd 
- arguments
    - key
- comments
    

#### getInt 
- arguments
    - key
    - default
- comments
    

#### getList 
- arguments
    - key
    - default
- comments
    

#### getListFromPrefix 
- arguments
    - prefix
- comments
    returns values from prefix return as list

#### getListFromPrefixEachItemDict 
- arguments
    - prefix
    - musthave = []
    - defaults = OrderedDict()
    - aredict = OrderedDict()
    - arelist = []
    - areint = []
    - arebool = []
- comments
    returns values from prefix return as list
    each value represents a dict
    @param musthave means for each item which is dict, we need to have following keys
    @param specifies the defaults
    @param aredicts & arelist specifies which types

#### getStr 
- arguments
    - key
    - default
- comments
    

#### listAdd 
- arguments
    - key
    - item
- comments
    

#### pop 
- arguments
    - key
- comments
    

#### prefix 
- arguments
    - key
    - depth = 0
- comments
    @param depth means prefix level to return

#### prefixexists 
- arguments
    - key
- comments
    

#### processall 
- arguments
- comments
    

#### set 
- arguments
    - key
    - val
    - persistent = True
- comments
    

