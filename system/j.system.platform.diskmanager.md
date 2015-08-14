## j.system.platform.diskmanager

- /opt/jumpscale7/lib/JumpScale/lib/diskmanager/Diskmanager.py

### def partitionsUnmount_Ext4Data() (l293)

### def partitionsFind(mounted=None,ttype=None,ssd=None,prefix="sd",minsize=5,maxsize=5000,devbusy=None,\ (l140)

looks for disks which are know to be data disks & are formatted ext4
return [[$partpath,$size,$free,$ssd]]
@param ssd if None then ssd and other

### def partitionsMount_Ext4Data() (l286)

### def mirrorsFind() (l135)

### def partitionsFind_Ext4Data() (l278)

looks for disks which are know to be data disks & are formatted ext4
return [[$partpath,$gid,$partid,$size,$free]]

### def diskGetFreeRegions(disk, align) (l123)

Get a filtered list of free regions, excluding the gaps due to partition alignment

### def partitionsGetMounted_Ext4Data() (l300)

find disks which are mounted
@return [[$partid,$size,$free]]

### def partitionAdd(disk, free, align=None, length=None, fs_type=None, type=None) (l93)

