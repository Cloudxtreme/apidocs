## j.clients.redisworker

- /opt/jumpscale7/lib/JumpScale/baselib/redisworker/RedisWorker.py
- Properties
    - sessionid
    - returnQueues

    

#### def checkJumpscriptQueue(jumpscript,queue) 

this checks that jumpscripts are not executed twice when being scheduled recurring
one off jobs will always execute !!!

#### def checkQueue() 

#### def deleteJob(jobid) 

#### def deleteJumpscripts() 

#### def deleteProcessQueue() 

#### def deleteQueues() 

#### def execFunction(method,_category="unknown", _organization="unknown",_timeout=60,_queue="default",_log=True,_sync=True,**args) 

@return job

#### def execJobAsync(job) 

#### def execJumpscript(jumpscriptid=None,jumpscript=None,_timeout=60,_queue="default",_log=True,_sync=True,**args) 

@return job

#### def getFailedJobs(queue=None, hoursago=0) 

#### def getJob(jobid) 

#### def getJobLine(job=None,jobid=None) 

#### def getJumpscriptFromId(jscriptid) 

#### def getJumpscriptFromName(organization,name) 

#### def getQueuedJobs(queue=None, asWikiTable=True) 

#### def removeJobs(hoursago=48, failed=False) 

#### def scheduleJob(job) 

#### def waitJob(job,timeout=600) 

