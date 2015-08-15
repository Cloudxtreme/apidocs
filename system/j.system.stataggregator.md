## j.system.stataggregator

- /opt/jumpscale7/lib/JumpScale/baselib/stataggregator/StatAggregator.py
- Properties
    - stats
    - log

### Methods

#### def clean 

##### arguments

#### def delete 

##### arguments

- prefix

#### def get 

##### arguments

- key

#### def getAvgMax 

##### arguments

- key

#### def getTime 

##### arguments

#### def list 

##### arguments

- prefix = ''
- memonly = False
- avgmax = False

#### def loadStat 

##### arguments

- key
- data

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

#### def send2log 

##### arguments

- name
- key
- val

#### def set 

##### arguments

- key
- val
- ttype = 'N'
- remember = True
- memonly = False
- percent = False

