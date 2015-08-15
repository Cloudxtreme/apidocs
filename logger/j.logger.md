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

#### def connectRedis 
##### arguments

##### comments

```

```

#### def disable 
##### arguments

##### comments

```

```

#### def getLogObjectFromDict 
##### arguments

- ddict

##### comments

```

```

#### def init 
##### arguments

##### comments

```

```

#### def log 
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

```
send to all log targets

```

#### def nologger 
##### arguments

- func

##### comments

```
Decorator to disable logging for a specific method (probably not thread safe)

```

#### def nostdout 
##### arguments

##### comments

```

```

#### def reset 
##### arguments

##### comments

```

```

