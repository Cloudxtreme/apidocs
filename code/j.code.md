## j.code

- /opt/jumpscale7/lib/JumpScale/baselib/code/Code.py

### Methods

#### def classEditGeany 

##### arguments

- classs

##### comments

```
look for editor (uses geany) and then edit the file

```

#### def classEditWing 

##### arguments

- classs

##### comments

```
look for editor (uses geany) and then edit the file

```

#### def classGetBase 

##### arguments

#### def classGetJSModelBase 

##### arguments

#### def classGetJSRootModelBase 

##### arguments

#### def classInfoGet 

##### arguments

- classs

##### comments

```
returns filepath,linenr,sourcecode

```

#### def classInfoPrint 

##### arguments

- classs

##### comments

```
print info like source code of class

```

#### def deIndent 

##### arguments

- content
- level = 1

#### def dict2JSModelobject 

##### arguments

- obj
- data

#### def dict2object 

##### arguments

- obj
- data

#### def indent 

##### arguments

- content
- level = 1

#### def object2dict 

##### arguments

- obj
- dieOnUnknown = False
- ignoreKeys = []
- ignoreUnderscoreKeys = False

#### def object2dict4index 

##### arguments

- obj

##### comments

```
convert object to a dict
only properties on first level are considered
and properties of basic types like int,str,float,bool,dict,list
ideal to index the basics of an object

```

#### def object2json 

##### arguments

- obj
- pretty = False
- skiperrors = False
- ignoreKeys = []
- ignoreUnderscoreKeys = False

#### def object2yaml 

##### arguments

- obj

#### def pprint 

##### arguments

- obj

