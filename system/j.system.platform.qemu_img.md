    #### def info(fileName, diskImageFormat=None, chain=False, unit='K') 
    
    Give information about the disk image <fileName>. Use it in particular to know the size reserved on
    disk which can be different from the displayed size. If VM snapshots are stored in the disk image,
    they are displayed too.
    
    @param fileName: a disk image filename
    @param diskImageFormat: disk image format
    @result: dict with info in KB
