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

##### comments

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

@param maxram = MB of ram
slave example: (192.168.10.10,8888,asecret)   (ip,port,secret)

#### def deleteInstance 
##### arguments

- name

##### comments

#### def emptyAllInstances 
##### arguments

##### comments

#### def emptyInstance 
##### arguments

- name

##### comments

#### def getByInstance 
##### arguments

- instance
- gevent = False

##### comments

#### def getGeventRedisClient 
##### arguments

- ipaddr
- port
- fromcache = True
- password = ''

##### comments

#### def getGeventRedisQueue 
##### arguments

- ipaddr
- port
- name
- namespace = 'queues'
- fromcache = False

##### comments

#### def getPort 
##### arguments

- name

##### comments

#### def getProcessPids 
##### arguments

- name

##### comments

#### def getRedisClient 
##### arguments

- ipaddr
- port
- password = ''
- fromcache = True

##### comments

#### def getRedisQueue 
##### arguments

- ipaddr
- port
- name
- namespace = 'queues'
- fromcache = True

##### comments

#### def isRunning 
##### arguments

- name

##### comments

#### def startInstance 
##### arguments

- name

##### comments

#### def stopInstance 
##### arguments

- name

##### comments

