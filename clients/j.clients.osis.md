## j.clients.osis

- /opt/jumpscale7/lib/JumpScale/grid/osis/OSISFactory.py
- Properties
    - osisConnectionsCat
    - osisConnections

#### get 
- arguments
    - ipaddr
    - port = 5544
    - user
    - passwd
    - ssl = False
    - gevent = False
- comments
    

#### getByInstance 
- arguments
    - instance
    - ssl = False
    - gevent = False
    - die = True
- comments
    

#### getCategory 
- arguments
    - client
    - namespace
    - category
- comments
    how to use
    @param client: osiclient
    @param namespace: OSIS namespace
    @param category: OSIS category

#### getNamespace 
- arguments
    - namespace
    - client
- comments
    

