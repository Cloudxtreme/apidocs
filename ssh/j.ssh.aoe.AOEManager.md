## j.ssh.aoe.AOEManager

- /opt/jumpscale7/lib/JumpScale/lib/ssh/aoe/manager.py

#### def create(storpath, size=10) 

    Create and vdisk
    
    :storpath: is the full image path.
    :size: size in GB

#### def delete(path) 

    

#### def expose(storage, major, minor, inf) 

    Expose the given image on major:minor and interface
    
    :storage: the image path or vdisk
    :major: Major number (shelf)
    :minor: Minor number (slot)
    :inf: Network interface

#### def list(storpath="/mnt/disktargets/") 

    List all vdisks under this location.
    Note that all files in that directory are assumed to be valid images

#### def unexpose(storage) 

    Unexpose the storage

