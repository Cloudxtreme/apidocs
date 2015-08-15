## j.logger

- /opt/jumpscale7/lib/JumpScale/core/logging/LogHandler.py
- Properties
    - nolog
    - redis
    - utils
    - enabled
    - consoleloglevel
    - lastmessage
    - redislogging
    - consolelogCategories
    - maxlevel

### Methods

#### connectRedis 
##### arguments

##### comments

#### disable 
##### arguments

##### comments

#### getLogObjectFromDict 
##### arguments

    - ddict

##### comments

#### init 
##### arguments

##### comments

#### log 
##### arguments

    - message
    - level = 5
    - category = ''
    - tags = ''
    - jid = ''
    - parentjid = ''
    - masterjid = ''
    - private = False

##### comments

send to all log targets

#### nologger 
##### arguments

    - func

##### comments

Decorator to disable logging for a specific method (probably not thread safe)

#### nostdout 
##### arguments

##### comments

#### reset 
##### arguments

##### comments

