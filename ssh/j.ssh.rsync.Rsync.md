## j.ssh.rsync.Rsync

- /opt/jumpscale7/lib/JumpScale/lib/ssh/rsync/manager.py

### Methods

#### def addModule 
##### arguments

- name

##### comments

add a module
mod = rsync.addModule('share')
mod.set('path', '/tmp/share')
rs.commit()

#### def commit 
##### arguments

##### comments

#### def erase 
##### arguments

##### comments

#### def removeModule 
##### arguments

- name

##### comments

#### def removeParams 
##### arguments

- key

##### comments

remove a global parameter

#### def restart 
##### arguments

##### comments

restart rsync daemon

#### def setParams 
##### arguments

- key
- value

##### comments

set a global parameter

#### def start 
##### arguments

##### comments

start rsync daemon

#### def stop 
##### arguments

##### comments

stop rsync daemon

