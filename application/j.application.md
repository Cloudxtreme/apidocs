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

### def getCPUUsage() (l272)

try to get cpu usage, if it doesn't work will return 0
By default 0 for windows

### def connectRedis() (l63)

### def initGrid() (l96)

### def getWhoAmiStr() (l102)

### def getAgentId() (l105)

### def stop(exitcode=0, stop=True) (l152)

Stop the application cleanly using a given exitcode

@param exitcode: Exit code to use
@type exitcode: number

### def getUniqueMachineId() (l321)

will look for network interface and return a hash calculated from lowest mac address from all physical nics

### def getAppInstanceHRD(name,instance,domain="jumpscale", parent=None) (l228)

returns hrd for specific domain,name and & instance name

### def start(name=None,appdir=".") (l110)

Start the application

You can only stop the application with return code 0 by calling
j.Application.stop(). Don't call sys.exit yourself, don't try to run
to end-of-script, I will find you anyway!

### def init() (l50)

### def initWhoAmI(reload=False) (l73)

when in grid:
    is gid,nid,pid

### def getMemoryUsage() (l296)

try to get memory usage, if it doesn't work will return 0i
By default 0 for windows

### def getAppHRDInstanceNames(name,domain="jumpscale") (l252)

returns hrd instance names for specific appname (default domain=jumpscale)

### def loadConfig() (l60)

### def getAppInstanceHRDs(name,domain="jumpscale") (l243)

returns list of hrd instances for specified app

### def existAppInstanceHRD(name,instance,domain="jumpscale") (l216)

returns hrd for specific appname & instance name (default domain=jumpscale or not used when inside a config git repo)

