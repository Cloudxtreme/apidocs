## j.clients.redisworker

- /opt/jumpscale7/lib/JumpScale/baselib/redisworker/RedisWorker.py
- Properties
    - sessionid
    - returnQueues

### Methods

    

#### def checkJumpscriptQueue 
##### arguments

- jumpscript
- queue

##### comments

this checks that jumpscripts are not executed twice when being scheduled recurring
one off jobs will always execute !!!

#### def checkQueue 
##### arguments

##### comments

#### def deleteJob 
##### arguments

- jobid

##### comments

#### def deleteJumpscripts 
##### arguments

##### comments

#### def deleteProcessQueue 
##### arguments

##### comments

#### def deleteQueues 
##### arguments

##### comments

#### def execFunction 
##### arguments

- method
- _category = 'unknown'
- _organization = 'unknown'
- _timeout = 60
- _queue = 'default'
- _log = True
- _sync = True
- **args

##### comments

@return job

#### def execJobAsync 
##### arguments

- job

##### comments

#### def execJumpscript 
##### arguments

- jumpscriptid
- jumpscript
- _timeout = 60
- _queue = 'default'
- _log = True
- _sync = True
- **args

##### comments

@return job

#### def getFailedJobs 
##### arguments

- queue
- hoursago = 0

##### comments

#### def getJob 
##### arguments

- jobid

##### comments

#### def getJobLine 
##### arguments

- job
- jobid

##### comments

#### def getJumpscriptFromId 
##### arguments

- jscriptid

##### comments

#### def getJumpscriptFromName 
##### arguments

- organization
- name

##### comments

#### def getQueuedJobs 
##### arguments

- queue
- asWikiTable = True

##### comments

#### def removeJobs 
##### arguments

- hoursago = 48
- failed = False

##### comments

#### def scheduleJob 
##### arguments

- job

##### comments

#### def waitJob 
##### arguments

- job
- timeout = 600

##### comments

