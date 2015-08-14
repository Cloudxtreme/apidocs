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

#### def connectRedis() 

#### def existAppInstanceHRD(name,instance,domain="jumpscale") 

returns hrd for specific appname & instance name (default domain=jumpscale or not used when inside a config git repo)

#### def getAgentId() 

#### def getAppHRDInstanceNames(name,domain="jumpscale") 

returns hrd instance names for specific appname (default domain=jumpscale)

#### def getAppInstanceHRD(name,instance,domain="jumpscale", parent=None) 

returns hrd for specific domain,name and & instance name

#### def getAppInstanceHRDs(name,domain="jumpscale") 

returns list of hrd instances for specified app

#### def getCPUUsage() 

try to get cpu usage, if it doesn't work will return 0
By default 0 for windows

#### def getMemoryUsage() 

try to get memory usage, if it doesn't work will return 0i
By default 0 for windows

#### def getUniqueMachineId() 

will look for network interface and return a hash calculated from lowest mac address from all physical nics

#### def getWhoAmiStr() 

#### def init() 

#### def initGrid() 

#### def initWhoAmI(reload=False) 

when in grid:
    is gid,nid,pid

#### def loadConfig() 

#### def start(name=None,appdir=".") 

Start the application

You can only stop the application with return code 0 by calling
j.Application.stop(). Don't call sys.exit yourself, don't try to run
to end-of-script, I will find you anyway!

#### def stop(exitcode=0, stop=True) 

Stop the application cleanly using a given exitcode

@param exitcode: Exit code to use
@type exitcode: number

