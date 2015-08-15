## j.ssh.rsync.Rsync

- /opt/jumpscale7/lib/JumpScale/lib/ssh/rsync/manager.py

### Methods

#### addModule 
##### arguments

    - name

##### comments

add a module
mod = rsync.addModule('share')
mod.set('path', '/tmp/share')
rs.commit()

#### commit 
##### arguments

##### comments

#### erase 
##### arguments

##### comments

#### removeModule 
##### arguments

    - name

##### comments

#### removeParams 
##### arguments

    - key

##### comments

remove a global parameter

#### restart 
##### arguments

##### comments

restart rsync daemon

#### setParams 
##### arguments

    - key
    - value

##### comments

set a global parameter

#### start 
##### arguments

##### comments

start rsync daemon

#### stop 
##### arguments

##### comments

stop rsync daemon

