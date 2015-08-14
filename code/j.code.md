## j.code

- /opt/jumpscale7/lib/JumpScale/baselib/code/Code.py

### def object2yaml(obj) (l273)

### def classInfoGet(classs) (l39)

returns filepath,linenr,sourcecode

### def classEditWing(classs) (l55)

look for editor (uses geany) and then edit the file

### def classGetJSRootModelBase() (l69)

### def object2dict(obj,dieOnUnknown=False,ignoreKeys=[],ignoreUnderscoreKeys=False) (l218)

### def pprint(obj) (l283)

### def dict2object(obj,data) (l81)

### def classInfoPrint(classs) (l31)

print info like source code of class

### def indent(content,level=1) (l293)

### def classGetBase() (l63)

### def object2json(obj,pretty=False,skiperrors=False,ignoreKeys=[],ignoreUnderscoreKeys=False) (l276)

### def dict2JSModelobject(obj,data) (l123)

### def deIndent(content,level=1) (l288)

### def classGetJSModelBase() (l66)

### def classEditGeany(classs) (l48)

look for editor (uses geany) and then edit the file

### def object2dict4index(obj) (l180)

convert object to a dict
only properties on first level are considered
and properties of basic types like int,str,float,bool,dict,list
ideal to index the basics of an object

