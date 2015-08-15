<!-- toc -->
## j.servers.geventws

- /opt/jumpscale7/lib/JumpScale/grid/geventws/GeventWSFactory.py
- Properties
    - cachecat
    - cache

### Methods

#### def getClient 

##### arguments

- addr
- port
- category = 'core'
- org = 'myorg'
- user = 'root'
- passwd = 'passwd'
- ssl = False
- roles = []
- id
- timeout = 60

#### def getHAClient 

##### arguments

- connections
- category = 'core'
- org = 'myorg'
- user = 'root'
- passwd = 'passwd'
- ssl = False
- roles = []
- id
- timeout = 60
- reconnect = False

#### def getServer 

##### arguments

- port
- sslorg
- ssluser
- sslkeyvaluestor

##### comments

```
HOW TO USE:
daemon=j.servers.geventws.getServer(port=4444)

class MyCommands():
    def __init__(self,daemon):
        self.daemon=daemon

    #session always needs to be there
    def pingcmd(self,session=session):
        return "pong"

    def echo(self,msg="",session=session):
        return msg

daemon.addCMDsInterface(MyCommands,category="optional")  #pass as class not as object !!!
    chose category if only 1 then can leave ""

daemon.start()

```

#### def initSSL4Server 

##### arguments

- organization
- serveruser
- sslkeyvaluestor

##### comments

```
use this to init your ssl keys for the server (they can be used over all transports)

```

