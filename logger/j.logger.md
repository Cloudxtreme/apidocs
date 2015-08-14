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

#### def connectRedis() 

#### def disable() 

#### def getLogObjectFromDict(ddict) 

#### def init() 

#### def log(message, level=5, category="", tags="", jid="", parentjid="",masterjid="", private=False) 

send to all log targets

#### def nologger(func) 

Decorator to disable logging for a specific method (probably not thread safe)

#### def nostdout() 

#### def reset() 

