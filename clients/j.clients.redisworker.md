## j.clients.redisworker

- /opt/jumpscale7/lib/JumpScale/baselib/redisworker/RedisWorker.py
- Properties
    - sessionid
    - returnQueues

    

### def execJobAsync(job) (l256)

### def getJob(jobid) (l126)

### def removeJobs(hoursago=48, failed=False) (l379)

### def execJumpscript(jumpscriptid=None,jumpscript=None,_timeout=60,_queue="default",_log=True,_sync=True,**args) (l231)

@return job

### def deleteQueues() (l148)

### def checkJumpscriptQueue(jumpscript,queue) (l214)

this checks that jumpscripts are not executed twice when being scheduled recurring
one off jobs will always execute !!!

### def deleteProcessQueue() (l152)

### def scheduleJob(job) (l328)

### def getQueuedJobs(queue=None, asWikiTable=True) (l345)

### def deleteJob(jobid) (l398)

### def deleteJumpscripts() (l144)

### def execFunction(method,_category="unknown", _organization="unknown",_timeout=60,_queue="default",_log=True,_sync=True,**args) (l165)

@return job

### def getJobLine(job=None,jobid=None) (l332)

### def getFailedJobs(queue=None, hoursago=0) (l359)

### def checkQueue() (l262)

### def getJumpscriptFromName(organization,name) (l156)

### def getJumpscriptFromId(jscriptid) (l135)

### def waitJob(job,timeout=600) (l294)

