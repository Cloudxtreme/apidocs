## j.application

- /opt/jumpscale7/lib/JumpScale/core/Application.py
- Properties
    - jid
    - appname
    - skipTraceback
    - whoAmIBytestr
    - redis
    - gridInitialized
    - sandbox
    - state
    - systempid
    - shellconfig
    - debug
    - agentid
    - config
    - whoAmI
    - interactive

### Methods

#### def connectRedis 
##### arguments

##### comments

#### def existAppInstanceHRD 
##### arguments

- name
- instance
- domain = 'jumpscale'

##### comments

returns hrd for specific appname & instance name (default domain=jumpscale or not used when inside a config git repo)

#### def getAgentId 
##### arguments

##### comments

#### def getAppHRDInstanceNames 
##### arguments

- name
- domain = 'jumpscale'

##### comments

returns hrd instance names for specific appname (default domain=jumpscale)

#### def getAppInstanceHRD 
##### arguments

- name
- instance
- domain = 'jumpscale'
- parent

##### comments

returns hrd for specific domain,name and & instance name

#### def getAppInstanceHRDs 
##### arguments

- name
- domain = 'jumpscale'

##### comments

returns list of hrd instances for specified app

#### def getCPUUsage 
##### arguments

##### comments

try to get cpu usage, if it doesn't work will return 0
By default 0 for windows

#### def getMemoryUsage 
##### arguments

##### comments

try to get memory usage, if it doesn't work will return 0i
By default 0 for windows

#### def getUniqueMachineId 
##### arguments

##### comments

will look for network interface and return a hash calculated from lowest mac address from all physical nics

#### def getWhoAmiStr 
##### arguments

##### comments

#### def init 
##### arguments

##### comments

#### def initGrid 
##### arguments

##### comments

#### def initWhoAmI 
##### arguments

- reload = False

##### comments

when in grid:
    is gid,nid,pid

#### def loadConfig 
##### arguments

##### comments

#### def start 
##### arguments

- name
- appdir = '.'

##### comments

Start the application

You can only stop the application with return code 0 by calling
j.Application.stop(). Don't call sys.exit yourself, don't try to run
to end-of-script, I will find you anyway!

#### def stop 
##### arguments

- exitcode = 0
- stop = True

##### comments

Stop the application cleanly using a given exitcode

@param exitcode: Exit code to use
@type exitcode: number

