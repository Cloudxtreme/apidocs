## j.clients.redis

- /opt/jumpscale7/lib/JumpScale/baselib/redis/Redis.py
- Properties
    - redisq
    - gredis
    - redis
    - gredisq

### Methods

    

#### def checkAllInstances 

##### arguments

#### def configureInstance 

##### arguments

- name
- port
- maxram = 200
- appendonly = True
- snapshot = False
- slave = ()
- ismaster = False
- passwd
- unixsocket = False

##### comments

```
@param maxram = MB of ram
slave example: (192.168.10.10,8888,asecret)   (ip,port,secret)

```

#### def deleteInstance 

##### arguments

- name

#### def emptyAllInstances 

##### arguments

#### def emptyInstance 

##### arguments

- name

#### def getByInstance 

##### arguments

- instance
- gevent = False

#### def getGeventRedisClient 

##### arguments

- ipaddr
- port
- fromcache = True
- password = ''

#### def getGeventRedisQueue 

##### arguments

- ipaddr
- port
- name
- namespace = 'queues'
- fromcache = False

#### def getPort 

##### arguments

- name

#### def getProcessPids 

##### arguments

- name

#### def getRedisClient 

##### arguments

- ipaddr
- port
- password = ''
- fromcache = True

#### def getRedisQueue 

##### arguments

- ipaddr
- port
- name
- namespace = 'queues'
- fromcache = True

#### def isRunning 

##### arguments

- name

#### def startInstance 

##### arguments

- name

#### def stopInstance 

##### arguments

- name

