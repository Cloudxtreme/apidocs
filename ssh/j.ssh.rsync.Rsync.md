## j.ssh.rsync.Rsync

- /opt/jumpscale7/lib/JumpScale/lib/ssh/rsync/manager.py

    #### def addModule(name) 
    
    add a module
    mod = rsync.addModule('share')
    mod.set('path', '/tmp/share')
    rs.commit()
    #### def commit() 
    #### def erase() 
    #### def removeModule(name) 
    #### def removeParams(key) 
    
    remove a global parameter
    #### def restart() 
    
    restart rsync daemon
    #### def setParams(key, value) 
    
    set a global parameter
    #### def start() 
    
    start rsync daemon
    #### def stop() 
    
    stop rsync daemon
