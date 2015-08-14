## j.clients.osis

- /opt/jumpscale7/lib/JumpScale/grid/osis/OSISFactory.py
- Properties
    - osisConnectionsCat
    - osisConnections

#### def get(ipaddr=None, port=5544,user=None,passwd=None,ssl=False,gevent=False) 

#### def getByInstance(instance=None, ssl=False, gevent=False,die=True) 

#### def getCategory(client, namespace, category) 

how to use
@param client: osiclient
@param namespace: OSIS namespace
@param category: OSIS category

#### def getNamespace(namespace, client=None) 

