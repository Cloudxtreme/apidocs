## j.base.idgenerator

- /opt/jumpscale7/lib/JumpScale/core/base/idgenerator/IDGenerator.py

generic provider of id's
lives at j.idgenerator

#### generateGUID 
- arguments
- comments
    generate unique guid
    how to use:  j.base.idgenerator.generateGUID()

#### generateIncrID 
- arguments
    - incrTypeId
    - service
    - reset = False
- comments
    type is like agent, job, jobstep
    needs to be a unique type, can only work if application service is known
    how to use:  j.base.idgenerator.generateIncrID("agent")
    @reset if True means restart from 1

#### generateRandomInt 
- arguments
    - fromInt
    - toInt
- comments
    how to use:  j.base.idgenerator.generateRandomInt(0,10)

#### generateXCharID 
- arguments
    - x
- comments
    

#### getID 
- arguments
    - incrTypeId
    - objectUniqueSeedInfo
    - service
    - reset = False
- comments
    get a unique id for an object uniquely identified
    remembers previously given id's

