## j.code

- /opt/jumpscale7/lib/JumpScale/baselib/code/Code.py

    #### def classEditGeany(classs) 
    
    look for editor (uses geany) and then edit the file
    #### def classEditWing(classs) 
    
    look for editor (uses geany) and then edit the file
    #### def classGetBase() 
    #### def classGetJSModelBase() 
    #### def classGetJSRootModelBase() 
    #### def classInfoGet(classs) 
    
    returns filepath,linenr,sourcecode
    #### def classInfoPrint(classs) 
    
    print info like source code of class
    #### def deIndent(content,level=1) 
    #### def dict2JSModelobject(obj,data) 
    #### def dict2object(obj,data) 
    #### def indent(content,level=1) 
    #### def object2dict(obj,dieOnUnknown=False,ignoreKeys=[],ignoreUnderscoreKeys=False) 
    #### def object2dict4index(obj) 
    
    convert object to a dict
    only properties on first level are considered
    and properties of basic types like int,str,float,bool,dict,list
    ideal to index the basics of an object
    #### def object2json(obj,pretty=False,skiperrors=False,ignoreKeys=[],ignoreUnderscoreKeys=False) 
    #### def object2yaml(obj) 
    #### def pprint(obj) 
