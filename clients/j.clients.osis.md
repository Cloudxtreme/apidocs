## j.clients.osis

- /opt/jumpscale7/lib/JumpScale/grid/osis/OSISFactory.py
- Properties
    - osisConnectionsCat
    - osisConnections

### Methods

#### def get 

##### arguments

- ipaddr
- port = 5544
- user
- passwd
- ssl = False
- gevent = False

#### def getByInstance 

##### arguments

- instance
- ssl = False
- gevent = False
- die = True

#### def getCategory 

##### arguments

- client
- namespace
- category

##### comments

```
how to use
@param client: osiclient
@param namespace: OSIS namespace
@param category: OSIS category

```

#### def getNamespace 

##### arguments

- namespace
- client

