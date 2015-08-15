## j.clients.portal

- /opt/jumpscale7/lib/JumpScale/portal/portal/PortalFactory.py

#### get 
- arguments
    - ip = 'localhost'
    - port = 9900
    - secret
- comments
    return client to manipulate & access a running application server (out of process)
    caching is done so can call this as many times as required
    secret is normally configured from grid
    there is normally no need to use this method, use self.getActorClient in stead

#### get2 
- arguments
    - ip = 'localhost'
    - port = 82
    - secret
- comments
    

#### getByInstance 
- arguments
    - instance
- comments
    

