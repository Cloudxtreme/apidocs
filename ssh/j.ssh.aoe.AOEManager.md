## j.ssh.aoe.AOEManager

- /opt/jumpscale7/lib/JumpScale/lib/ssh/aoe/manager.py

### Methods

#### def create 

##### arguments

- storpath
- size = 10

##### comments

```
Create and vdisk

:storpath: is the full image path.
:size: size in GB

```

#### def delete 

##### arguments

- path

#### def expose 

##### arguments

- storage
- major
- minor
- inf

##### comments

```
Expose the given image on major:minor and interface

:storage: the image path or vdisk
:major: Major number (shelf)
:minor: Minor number (slot)
:inf: Network interface

```

#### def list 

##### arguments

- storpath = '/mnt/disktargets/'

##### comments

```
List all vdisks under this location.
Note that all files in that directory are assumed to be valid images

```

#### def unexpose 

##### arguments

- storage

##### comments

```
Unexpose the storage

```

