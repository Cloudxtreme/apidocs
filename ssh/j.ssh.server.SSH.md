## j.ssh.server.SSH

- /opt/jumpscale7/lib/JumpScale/lib/ssh/server/manager.py

### Methods

#### addKey 
##### arguments

    - key

##### comments

Add pubkey to authorized_keys

#### commit 
##### arguments

##### comments

Apply all pending changes to authorized_keys

#### deleteKey 
##### arguments

    - key

##### comments

Delete pubkey from authorized_keys

#### disableNonKeyAccess 
##### arguments

##### comments

Disable passowrd login to server. This action doens't require
calling to commit and applies immediately. So if you added your key
make sure to commit it before you call this method.

#### erase 
##### arguments

##### comments

Erase all keys from authorized_keys

