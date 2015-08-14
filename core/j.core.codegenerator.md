## j.core.codegenerator

- /opt/jumpscale7/lib/JumpScale/baselib/codegentools/CodeGenerator.py
- Properties
    - appdir
    - codepath
    - classes
    - generated

### def getClassActorLocal(appname, actor, typecheck=True, dieInGenCode=True) (l62)

### def getActorClass(appname, actor, typecheck=True, dieInGenCode=True, codepath=None) (l75)

### def getClassActorRemote(appname, actor, typecheck=True, dieInGenCode=True, instance=0, redis=False, wsclient=None, codepath=None) (l89)

### def getCodeJSModel(appname, actor, modelname, typecheck=True, dieInGenCode=True, codepath="") (l129)

### def setTarget(target) (l29)

Sets the target to generate for server or client

### def getClassesActorMethodGreenlet(appname, actor, typecheck=True, dieInGenCode=True) (l101)

return: returns dict with key name methodname and then the class (for each method a class is generated)

### def removeFromMem(appname, actor) (l35)

### def getCodeId(spec, type) (l174)

### def getCodeEveModel(appname, actor, modelname, typecheck=True, dieInGenCode=True, codepath="") (l139)

### def getClassJSModel(appname, actor, modelname, typecheck=True, dieInGenCode=True, codepath="") (l115)

### def getClassEnumeration(appname, actor, enumname, typecheck=True, dieInGenCode=True) (l162)

### def resetMemNonSystem() (l51)

### def generate(spec, type, typecheck=True, dieInGenCode=True, appserverclient=None, instance=0, redis=False, wsclient=None, (l177)

param: spec is spec we want to generate from
param: type JSModel,actormethodgreenlet,enumeration,actorlocal
param: typecheck (means in generated code the types will be checked)
param: dieInGenCode  if true means in generated code we will die when something uneforeseen happens
return: dict of classes if more than 1 otherwise just the class

