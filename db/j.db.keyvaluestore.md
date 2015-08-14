    #### def getRedisStore(namespace='',host='localhost',port=9999,db=0,password='',serializers=None,masterdb=None,changelog=True) 
    
    Gets a memory key value store.
    
    @param name: name of the store
    @type name: String
    
    @param namespace: namespace of the store, defaults to None
    @type namespace: String
    
    @return: key value store
    @rtype: MemoryKeyValueStore
