## j.clients.portal

- /opt/jumpscale7/lib/JumpScale/portal/portal/PortalFactory.py

### def get2(ip="localhost", port=82, secret=None) (l48)

### def getByInstance(instance=None) (l20)

### def get(ip="localhost", port=9900, secret=None) (l29)

return client to manipulate & access a running application server (out of process)
caching is done so can call this as many times as required
secret is normally configured from grid
there is normally no need to use this method, use self.getActorClient in stead

