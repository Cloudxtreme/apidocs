## j.core.codegenerator

- /opt/jumpscale7/lib/JumpScale/baselib/codegentools/CodeGenerator.py
- Properties
    - appdir
    - codepath
    - classes
    - generated

#### def generate(spec, type, typecheck=True, dieInGenCode=True, appserverclient=None, instance=0, redis=False, wsclient=None, 

    param: spec is spec we want to generate from
    param: type JSModel,actormethodgreenlet,enumeration,actorlocal
    param: typecheck (means in generated code the types will be checked)
    param: dieInGenCode  if true means in generated code we will die when something uneforeseen happens
    return: dict of classes if more than 1 otherwise just the class

#### def getActorClass(appname, actor, typecheck=True, dieInGenCode=True, codepath=None) 

    

#### def getClassActorLocal(appname, actor, typecheck=True, dieInGenCode=True) 

    

#### def getClassActorRemote(appname, actor, typecheck=True, dieInGenCode=True, instance=0, redis=False, wsclient=None, codepath=None) 

    

#### def getClassEnumeration(appname, actor, enumname, typecheck=True, dieInGenCode=True) 

    

#### def getClassJSModel(appname, actor, modelname, typecheck=True, dieInGenCode=True, codepath="") 

    

#### def getClassesActorMethodGreenlet(appname, actor, typecheck=True, dieInGenCode=True) 

    return: returns dict with key name methodname and then the class (for each method a class is generated)

#### def getCodeEveModel(appname, actor, modelname, typecheck=True, dieInGenCode=True, codepath="") 

    

#### def getCodeId(spec, type) 

    

#### def getCodeJSModel(appname, actor, modelname, typecheck=True, dieInGenCode=True, codepath="") 

    

#### def removeFromMem(appname, actor) 

    

#### def resetMemNonSystem() 

    

#### def setTarget(target) 

    Sets the target to generate for server or client

