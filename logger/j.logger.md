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

### def reset() (l233)

### def connectRedis() (l168)

### def log(message, level=5, category="", tags="", jid="", parentjid="",masterjid="", private=False) (l248)

send to all log targets

### def nostdout() (l206)

### def init() (l164)

### def disable() (l242)

### def nologger(func) (l193)

Decorator to disable logging for a specific method (probably not thread safe)

### def getLogObjectFromDict(ddict) (l190)

