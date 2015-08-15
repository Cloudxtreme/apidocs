## j.clients.mercurial

- /opt/jumpscale7/lib/JumpScale/baselib/mercurial/HgLibFactory.py

### Methods

#### def getClient 
##### arguments

- hgbasedir
- remoteUrl = ''
- branchname
- cleandir = False

##### comments

```
return a mercurial tool which you can help to manipulate a hg repository
@param base dir where local hgrepository will be stored
@branchname "" means is the tip, None means will try to fetch the branchname from the basedir
@param remote url of hg repository, e.g. https://login:passwd@bitbucket.org/despiegk/ssospecs/  #DO NOT FORGET LOGIN PASSWD

```

#### def log 
##### arguments

- msg
- category = ''
- level = 5

##### comments

```

```

