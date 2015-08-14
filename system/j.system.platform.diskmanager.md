## j.system.platform.diskmanager

- /opt/jumpscale7/lib/JumpScale/lib/diskmanager/Diskmanager.py

#### def diskGetFreeRegions(disk, align) 

Get a filtered list of free regions, excluding the gaps due to partition alignment

#### def mirrorsFind() 

#### def partitionAdd(disk, free, align=None, length=None, fs_type=None, type=None) 

#### def partitionsFind(mounted=None,ttype=None,ssd=None,prefix="sd",minsize=5,maxsize=5000,devbusy=None,\ 

looks for disks which are know to be data disks & are formatted ext4
return [[$partpath,$size,$free,$ssd]]
@param ssd if None then ssd and other

#### def partitionsFind_Ext4Data() 

looks for disks which are know to be data disks & are formatted ext4
return [[$partpath,$gid,$partid,$size,$free]]

#### def partitionsGetMounted_Ext4Data() 

find disks which are mounted
@return [[$partid,$size,$free]]

#### def partitionsMount_Ext4Data() 

#### def partitionsUnmount_Ext4Data() 

