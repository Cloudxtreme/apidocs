## j.clients.redis

- /opt/jumpscale7/lib/JumpScale/baselib/redis/Redis.py
- Properties
    - redisq
    - gredis
    - redis
    - gredisq

    

#### checkAllInstances 
- arguments
- comments
    

#### configureInstance 
- arguments
    - name
    - port
    - maxram = 200
    - appendonly = True
    - snapshot = False
    - slave = ()
    - ismaster = False
    - passwd
    - unixsocket = False
- comments
    @param maxram = MB of ram
    slave example: (192.168.10.10,8888,asecret)   (ip,port,secret)

#### deleteInstance 
- arguments
    - name
- comments
    

#### emptyAllInstances 
- arguments
- comments
    

#### emptyInstance 
- arguments
    - name
- comments
    

#### getByInstance 
- arguments
    - instance
    - gevent = False
- comments
    

#### getGeventRedisClient 
- arguments
    - ipaddr
    - port
    - fromcache = True
    - password = ''
- comments
    

#### getGeventRedisQueue 
- arguments
    - ipaddr
    - port
    - name
    - namespace = 'queues'
    - fromcache = False
- comments
    

#### getPort 
- arguments
    - name
- comments
    

#### getProcessPids 
- arguments
    - name
- comments
    

#### getRedisClient 
- arguments
    - ipaddr
    - port
    - password = ''
    - fromcache = True
- comments
    

#### getRedisQueue 
- arguments
    - ipaddr
    - port
    - name
    - namespace = 'queues'
    - fromcache = True
- comments
    

#### isRunning 
- arguments
    - name
- comments
    

#### startInstance 
- arguments
    - name
- comments
    

#### stopInstance 
- arguments
    - name
- comments
    

