## j.system.btrfs

- /opt/jumpscale7/lib/JumpScale/lib/btrfs/BtrfsExtension.py

#### def deviceAdd(path, dev) 

Add a device to a filesystem.

#### def deviceDelete(dev, path) 

Remove a device from a filesystem.

#### def getSpaceUsage(path) 

#### def snapshotReadOnlyCreate(path, dest) 

Create a readonly snapshot

#### def subvolumeCreate(path, name) 

Create a subvolume in <dest> (or the current directory if not passed).

#### def subvolumeDelete(path, name) 

Delete the subvolume <name>.

#### def subvolumeList(path) 

List the snapshot/subvolume of a filesystem.

