## j.remote.system

- /opt/jumpscale7/lib/JumpScale/baselib/remote/remotesystem/RemoteSystem.py
- Properties
    - connections

#### def connect(ip, login="", password="", timeout=120.0, port=22) 

Creates a connection object to a remote system via ssh.

@param ip: Ipaddress of the remote system
@param login: Username used for login on remote system
@param password: Password used for login on remote system
@param timeout: Timeout for the SSH session       
@rtype: RemoteSystemConnection

