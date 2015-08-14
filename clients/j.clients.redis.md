## j.clients.redis

- /opt/jumpscale7/lib/JumpScale/baselib/redis/Redis.py
- Properties
    - redisq
    - gredis
    - redis
    - gredisq

    

### def emptyAllInstances() (l142)

### def startInstance(name) (l199)

### def isRunning(name) (l164)

### def emptyInstance(name) (l207)

### def getGeventRedisClient(ipaddr, port, fromcache=True,password="") (l82)

### def getRedisClient(ipaddr, port, password="", fromcache=True) (l92)

### def stopInstance(name) (l192)

### def getGeventRedisQueue(ipaddr, port, name, namespace="queues", fromcache=False) (l122)

### def getProcessPids(name) (l179)

### def configureInstance(name, port, maxram=200, appendonly=True,snapshot=False,slave=(),ismaster=False,passwd=None,unixsocket=False) (l214)

@param maxram = MB of ram
slave example: (192.168.10.10,8888,asecret)   (ip,port,secret)

### def deleteInstance(name) (l202)

### def checkAllInstances() (l131)

### def getRedisQueue(ipaddr, port, name, namespace="queues", fromcache=True) (l114)

### def getPort(name) (l155)

### def getByInstance(instance, gevent=False) (l100)

