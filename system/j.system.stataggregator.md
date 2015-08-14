## j.system.stataggregator

- /opt/jumpscale7/lib/JumpScale/baselib/stataggregator/StatAggregator.py
- Properties
    - stats
    - log

### def send2carbon() (l226)

### def set(key,val,ttype="N",remember=True,memonly=False,percent=False) (l158)

### def get(key) (l171)

### def getTime() (l121)

### def send2log(name,key,val) (l124)

### def getAvgMax(key) (l176)

### def list(prefix="",memonly=False,avgmax=False) (l209)

### def loadStat(key=None, data=None) (l148)

### def registerStats(key,ttype="N",memonly=False,percent=False) (l181)

type is N or D (D from diff)

### def clean() (l193)

### def delete(prefix) (l202)

