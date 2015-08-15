<!-- toc -->
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

```
this checks that jumpscripts are not executed twice when being scheduled recurring
one off jobs will always execute !!!

```

#### def checkQueue 

##### arguments

#### def deleteJob 

##### arguments

- jobid

#### def deleteJumpscripts 

##### arguments

#### def deleteProcessQueue 

##### arguments

#### def deleteQueues 

##### arguments

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

```
@return job

```

#### def execJobAsync 

##### arguments

- job

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

```
@return job

```

#### def getFailedJobs 

##### arguments

- queue
- hoursago = 0

#### def getJob 

##### arguments

- jobid

#### def getJobLine 

##### arguments

- job
- jobid

#### def getJumpscriptFromId 

##### arguments

- jscriptid

#### def getJumpscriptFromName 

##### arguments

- organization
- name

#### def getQueuedJobs 

##### arguments

- queue
- asWikiTable = True

#### def removeJobs 

##### arguments

- hoursago = 48
- failed = False

#### def scheduleJob 

##### arguments

- job

#### def waitJob 

##### arguments

- job
- timeout = 600

