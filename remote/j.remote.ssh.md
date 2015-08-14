## j.remote.ssh

- /opt/jumpscale7/lib/JumpScale/baselib/remote/ssh/SSHTool.py

    #### def getSSHClient(password,  host="localhost", username="root", port=22,timeout=10) 
    
    Create a new SSHClient instance.
    
    @param host: Hostname to connect to
    @type host: string
    @param username: Username to connect as
    @type username: string
    @param password: Password to authenticate with
    @type password: string
    @param timeout: Connection timeout
    @type timeout: number
    
    @return: SSHClient instance
    @rtype: SSHClient
    #### def getSSHClientUsingKey(keypath,host="localhost",username="root",port=22,timeout=10) 
    
    Create a new SSHClient instance.
    @return: SSHClient instance
    @rtype: SSHClient
    #### def getSSHClientUsingSSHAgent(host="localhost",username="root",port=22,timeout=10) 
    
    Create a new SSHClient instance using ssh agent.
