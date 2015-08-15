## j.system.btrfs

- /opt/jumpscale7/lib/JumpScale/lib/btrfs/BtrfsExtension.py

### Methods

#### def deviceAdd 

##### arguments

- path
- dev

##### comments

```
Add a device to a filesystem.

```

#### def deviceDelete 

##### arguments

- dev
- path

##### comments

```
Remove a device from a filesystem.

```

#### def getSpaceUsage 

##### arguments

- path

#### def snapshotReadOnlyCreate 

##### arguments

- path
- dest

##### comments

```
Create a readonly snapshot

```

#### def subvolumeCreate 

##### arguments

- path
- name

##### comments

```
Create a subvolume in <dest> (or the current directory if not passed).

```

#### def subvolumeDelete 

##### arguments

- path
- name

##### comments

```
Delete the subvolume <name>.

```

#### def subvolumeList 

##### arguments

- path

##### comments

```
List the snapshot/subvolume of a filesystem.

```

