## j.db.keyvaluestore

- /opt/jumpscale7/lib/JumpScale/baselib/key_value_store/store_factory.py

The key value store factory provides logic to retrieve store instances. It
also caches the stores based on their type, name and namespace.

### def getMemoryStore(namespace=None) (l81)

Gets a memory key value store.

@return: key value store
@rtype: MemoryKeyValueStore

### def getLevelDBStore(namespace='',basedir=None,serializers=[]) (l110)

Gets a leveldb key value store.

@param name: name of the store
@type name: String

@param namespace: namespace of the store, defaults to ''
@type namespace: String

@return: key value store

### def getArakoonStore(namespace='',serializers=[]) (l31)

Gets an Arakoon key value store.

@param namespace: namespace of the store, defaults to None
@type namespace: String

@param defaultJSModelSerializer: default JSModel serializer
@type defaultJSModelSerializer: Object

@return: key value store
@rtype: ArakoonKeyValueStore

### def getFileSystemStore(namespace='', baseDir=None,serializers=[]) (l54)

Gets a file system key value store.

@param namespace: namespace of the store, defaults to an empty string
@type namespace: String

@param baseDir: base directory of the store, defaults to j.dirs.db
@type namespace: String

@param defaultJSModelSerializer: default JSModel serializer
@type defaultJSModelSerializer: Object

@return: key value store
@rtype: FileSystemKeyValueStore

### def getRedisStore(namespace='',host='localhost',port=9999,db=0,password='',serializers=None,masterdb=None,changelog=True) (l91)

Gets a memory key value store.

@param name: name of the store
@type name: String

@param namespace: namespace of the store, defaults to None
@type namespace: String

@return: key value store
@rtype: MemoryKeyValueStore

