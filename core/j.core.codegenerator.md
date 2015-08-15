## j.core.codegenerator

- /opt/jumpscale7/lib/JumpScale/baselib/codegentools/CodeGenerator.py
- Properties
    - appdir
    - codepath
    - classes
    - generated

### Methods

#### def generate 
##### arguments

- spec
- type
- typecheck = True
- dieInGenCode = True
- appserverclient
- instance = 0
- redis = False
- wsclient
- codepath
- classpath
- returnClass = True
- args = \{\}
- makeCopy = False

##### comments

param: spec is spec we want to generate from
param: type JSModel,actormethodgreenlet,enumeration,actorlocal
param: typecheck (means in generated code the types will be checked)
param: dieInGenCode  if true means in generated code we will die when something uneforeseen happens
return: dict of classes if more than 1 otherwise just the class

#### def getActorClass 
##### arguments

- appname
- actor
- typecheck = True
- dieInGenCode = True
- codepath

##### comments

#### def getClassActorLocal 
##### arguments

- appname
- actor
- typecheck = True
- dieInGenCode = True

##### comments

#### def getClassActorRemote 
##### arguments

- appname
- actor
- typecheck = True
- dieInGenCode = True
- instance = 0
- redis = False
- wsclient
- codepath

##### comments

#### def getClassEnumeration 
##### arguments

- appname
- actor
- enumname
- typecheck = True
- dieInGenCode = True

##### comments

#### def getClassJSModel 
##### arguments

- appname
- actor
- modelname
- typecheck = True
- dieInGenCode = True
- codepath = ''

##### comments

#### def getClassesActorMethodGreenlet 
##### arguments

- appname
- actor
- typecheck = True
- dieInGenCode = True

##### comments

return: returns dict with key name methodname and then the class (for each method a class is generated)

#### def getCodeEveModel 
##### arguments

- appname
- actor
- modelname
- typecheck = True
- dieInGenCode = True
- codepath = ''

##### comments

#### def getCodeId 
##### arguments

- spec
- type

##### comments

#### def getCodeJSModel 
##### arguments

- appname
- actor
- modelname
- typecheck = True
- dieInGenCode = True
- codepath = ''

##### comments

#### def removeFromMem 
##### arguments

- appname
- actor

##### comments

#### def resetMemNonSystem 
##### arguments

##### comments

#### def setTarget 
##### arguments

- target

##### comments

Sets the target to generate for server or client

