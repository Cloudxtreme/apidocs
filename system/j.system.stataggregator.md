## j.system.stataggregator

- /opt/jumpscale7/lib/JumpScale/baselib/stataggregator/StatAggregator.py
- Properties
    - stats
    - log

    #### def clean() 
    #### def delete(prefix) 
    #### def get(key) 
    #### def getAvgMax(key) 
    #### def getTime() 
    #### def list(prefix="",memonly=False,avgmax=False) 
    #### def loadStat(key=None, data=None) 
    #### def registerStats(key,ttype="N",memonly=False,percent=False) 
    
    type is N or D (D from diff)
    #### def send2carbon() 
    #### def send2log(name,key,val) 
    #### def set(key,val,ttype="N",remember=True,memonly=False,percent=False) 
