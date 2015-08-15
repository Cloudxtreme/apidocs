## j.remote.ssh

- /opt/jumpscale7/lib/JumpScale/baselib/remote/ssh/SSHTool.py

### Methods

#### def getSSHClient 
##### arguments

- password
- host = 'localhost'
- username = 'root'
- port = 22
- timeout = 10

##### comments

```
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

```

#### def getSSHClientUsingKey 
##### arguments

- keypath
- host = 'localhost'
- username = 'root'
- port = 22
- timeout = 10

##### comments

```
Create a new SSHClient instance.
@return: SSHClient instance
@rtype: SSHClient

```

#### def getSSHClientUsingSSHAgent 
##### arguments

- host = 'localhost'
- username = 'root'
- port = 22
- timeout = 10

##### comments

```
Create a new SSHClient instance using ssh agent.

```

