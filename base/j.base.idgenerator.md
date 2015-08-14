## j.base.idgenerator

- /opt/jumpscale7/lib/JumpScale/core/base/idgenerator/IDGenerator.py

generic provider of id's
lives at j.idgenerator

### def getID(incrTypeId,objectUniqueSeedInfo,service,reset=False) (l34)

get a unique id for an object uniquely identified
remembers previously given id's

### def generateGUID() (l48)

generate unique guid
how to use:  j.base.idgenerator.generateGUID()

### def generateRandomInt(fromInt,toInt) (l12)

how to use:  j.base.idgenerator.generateRandomInt(0,10)

### def generateIncrID(incrTypeId,service,reset=False) (l18)

type is like agent, job, jobstep
needs to be a unique type, can only work if application service is known
how to use:  j.base.idgenerator.generateIncrID("agent")
@reset if True means restart from 1

### def generateXCharID(x) (l56)

