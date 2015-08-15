## j.system.stataggregator

- /opt/jumpscale7/lib/JumpScale/baselib/stataggregator/StatAggregator.py
- Properties
    - stats
    - log

#### clean 
- arguments
- comments
    

#### delete 
- arguments
    - prefix
- comments
    

#### get 
- arguments
    - key
- comments
    

#### getAvgMax 
- arguments
    - key
- comments
    

#### getTime 
- arguments
- comments
    

#### list 
- arguments
    - prefix = ''
    - memonly = False
    - avgmax = False
- comments
    

#### loadStat 
- arguments
    - key
    - data
- comments
    

#### registerStats 
- arguments
    - key
    - ttype = 'N'
    - memonly = False
    - percent = False
- comments
    type is N or D (D from diff)

#### send2carbon 
- arguments
- comments
    

#### send2log 
- arguments
    - name
    - key
    - val
- comments
    

#### set 
- arguments
    - key
    - val
    - ttype = 'N'
    - remember = True
    - memonly = False
    - percent = False
- comments
    

