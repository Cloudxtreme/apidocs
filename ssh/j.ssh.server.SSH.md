## j.ssh.server.SSH

- /opt/jumpscale7/lib/JumpScale/lib/ssh/server/manager.py

    #### def addKey(key) 
    
    Add pubkey to authorized_keys
    #### def commit() 
    
    Apply all pending changes to authorized_keys
    #### def deleteKey(key) 
    
    Delete pubkey from authorized_keys
    #### def disableNonKeyAccess() 
    
    Disable passowrd login to server. This action doens't require
    calling to commit and applies immediately. So if you added your key
    make sure to commit it before you call this method.
    #### def erase() 
    
    Erase all keys from authorized_keys
