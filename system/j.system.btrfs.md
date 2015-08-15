## j.system.btrfs

- /opt/jumpscale7/lib/JumpScale/lib/btrfs/BtrfsExtension.py

#### deviceAdd 
- arguments
    - path
    - dev
- comments
    Add a device to a filesystem.

#### deviceDelete 
- arguments
    - dev
    - path
- comments
    Remove a device from a filesystem.

#### getSpaceUsage 
- arguments
    - path
- comments
    

#### snapshotReadOnlyCreate 
- arguments
    - path
    - dest
- comments
    Create a readonly snapshot

#### subvolumeCreate 
- arguments
    - path
    - name
- comments
    Create a subvolume in <dest> (or the current directory if not passed).

#### subvolumeDelete 
- arguments
    - path
    - name
- comments
    Delete the subvolume <name>.

#### subvolumeList 
- arguments
    - path
- comments
    List the snapshot/subvolume of a filesystem.

