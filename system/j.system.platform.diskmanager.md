## j.system.platform.diskmanager

- /opt/jumpscale7/lib/JumpScale/lib/diskmanager/Diskmanager.py

### Methods

#### def diskGetFreeRegions 
##### arguments

- disk
- align

##### comments

```
Get a filtered list of free regions, excluding the gaps due to partition alignment

```

#### def mirrorsFind 
##### arguments

#### def partitionAdd 
##### arguments

- disk
- free
- align
- length
- fs_type
- type
#### def partitionsFind 
##### arguments

- mounted
- ttype
- ssd
- prefix = 'sd'
- minsize = 5
- maxsize = 5000
- devbusy
- initialize = False
- forceinitialize = False

##### comments

```
looks for disks which are know to be data disks & are formatted ext4
return [[$partpath,$size,$free,$ssd]]
@param ssd if None then ssd and other

```

#### def partitionsFind_Ext4Data 
##### arguments

##### comments

```
looks for disks which are know to be data disks & are formatted ext4
return [[$partpath,$gid,$partid,$size,$free]]

```

#### def partitionsGetMounted_Ext4Data 
##### arguments

##### comments

```
find disks which are mounted
@return [[$partid,$size,$free]]

```

#### def partitionsMount_Ext4Data 
##### arguments

#### def partitionsUnmount_Ext4Data 
##### arguments

