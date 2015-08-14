## j.clients.redis

- /opt/jumpscale7/lib/JumpScale/baselib/redis/Redis.py
- Properties
    - redisq
    - gredis
    - redis
    - gredisq

    

#### def checkAllInstances() 

#### def configureInstance(name, port, maxram=200, appendonly=True,snapshot=False,slave=(),ismaster=False,passwd=None,unixsocket=False) 

@param maxram = MB of ram
slave example: (192.168.10.10,8888,asecret)   (ip,port,secret)

#### def deleteInstance(name) 

#### def emptyAllInstances() 

#### def emptyInstance(name) 

#### def getByInstance(instance, gevent=False) 

#### def getGeventRedisClient(ipaddr, port, fromcache=True,password="") 

#### def getGeventRedisQueue(ipaddr, port, name, namespace="queues", fromcache=False) 

#### def getPort(name) 

#### def getProcessPids(name) 

#### def getRedisClient(ipaddr, port, password="", fromcache=True) 

#### def getRedisQueue(ipaddr, port, name, namespace="queues", fromcache=True) 

#### def isRunning(name) 

#### def startInstance(name) 

#### def stopInstance(name) 

