## j.system.stataggregator

- /opt/jumpscale7/lib/JumpScale/baselib/stataggregator/StatAggregator.py
- Properties
    - stats
    - log

### Methods

#### def clean 
##### arguments

##### comments

```

```

#### def delete 
##### arguments

- prefix

##### comments

```

```

#### def get 
##### arguments

- key

##### comments

```

```

#### def getAvgMax 
##### arguments

- key

##### comments

```

```

#### def getTime 
##### arguments

##### comments

```

```

#### def list 
##### arguments

- prefix = ''
- memonly = False
- avgmax = False

##### comments

```

```

#### def loadStat 
##### arguments

- key
- data

##### comments

```

```

#### def registerStats 
##### arguments

- key
- ttype = 'N'
- memonly = False
- percent = False

##### comments

```
type is N or D (D from diff)

```

#### def send2carbon 
##### arguments

##### comments

```

```

#### def send2log 
##### arguments

- name
- key
- val

##### comments

```

```

#### def set 
##### arguments

- key
- val
- ttype = 'N'
- remember = True
- memonly = False
- percent = False

##### comments

```

```

