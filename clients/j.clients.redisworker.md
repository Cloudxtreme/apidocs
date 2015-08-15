## j.clients.redisworker

- /opt/jumpscale7/lib/JumpScale/baselib/redisworker/RedisWorker.py
- Properties
    - sessionid
    - returnQueues

    

#### checkJumpscriptQueue 
- arguments
    - jumpscript
    - queue
- comments
    this checks that jumpscripts are not executed twice when being scheduled recurring
    one off jobs will always execute !!!

#### checkQueue 
- arguments
- comments
    

#### deleteJob 
- arguments
    - jobid
- comments
    

#### deleteJumpscripts 
- arguments
- comments
    

#### deleteProcessQueue 
- arguments
- comments
    

#### deleteQueues 
- arguments
- comments
    

#### execFunction 
- arguments
    - method
    - _category = 'unknown'
    - _organization = 'unknown'
    - _timeout = 60
    - _queue = 'default'
    - _log = True
    - _sync = True
    - **args
- comments
    @return job

#### execJobAsync 
- arguments
    - job
- comments
    

#### execJumpscript 
- arguments
    - jumpscriptid
    - jumpscript
    - _timeout = 60
    - _queue = 'default'
    - _log = True
    - _sync = True
    - **args
- comments
    @return job

#### getFailedJobs 
- arguments
    - queue
    - hoursago = 0
- comments
    

#### getJob 
- arguments
    - jobid
- comments
    

#### getJobLine 
- arguments
    - job
    - jobid
- comments
    

#### getJumpscriptFromId 
- arguments
    - jscriptid
- comments
    

#### getJumpscriptFromName 
- arguments
    - organization
    - name
- comments
    

#### getQueuedJobs 
- arguments
    - queue
    - asWikiTable = True
- comments
    

#### removeJobs 
- arguments
    - hoursago = 48
    - failed = False
- comments
    

#### scheduleJob 
- arguments
    - job
- comments
    

#### waitJob 
- arguments
    - job
    - timeout = 600
- comments
    

