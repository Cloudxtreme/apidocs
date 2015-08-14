## j.base.time

- /opt/jumpscale7/lib/JumpScale/core/base/time/Time.py

generic provider of time functions
lives at j.base.time

    #### def HRDatetoEpoch(datestr,local=True) 
    
    convert string date to epoch
    Date needs to be formatted as 16/06/1988
    #### def epoch2HRDate(epoch,local=True) 
    #### def epoch2HRDateTime(epoch,local=True) 
    #### def epoch2HRTime(epoch,local=True) 
    #### def fiveMinuteIdToEpoch(fiveMinuteId) 
    #### def formatTime(epoch,formatstr='%Y/%m/%d %H%M%S',local=True) 
    
    Returns a formatted time string representing the current time
    
    See http://docs.python.org/lib/module-time.html#l2h-2826 for an
    overview of available formatting options.
    
    @param format: Format string
    @type format: string
    
    @returns: Formatted current time
    @rtype: string
    #### def get5MinuteId(epoch=None) 
    
    is # 5 min from jan 1 2010
    #### def getDayId(epoch=None) 
    
    is # day from jan 1 2010
    #### def getDeltaTime(txt) 
    
    only supported now is -3m, -3d and -3h (ofcourse 3 can be any int)
    and an int which would be just be returned
    means 3 days ago 3 hours ago
    if 0 or '' then is now
    #### def getEpochAgo(txt) 
    
    only supported now is -3m, -3d and -3h  (ofcourse 3 can be any int)
    and an int which would be just be returned
    means 3 days ago 3 hours ago
    if 0 or '' then is now
    #### def getEpochFuture(txt) 
    
    only supported now is +3d and +3h  (ofcourse 3 can be any int)        
    +3d means 3 days in future
    and an int which would be just be returned
    if txt==None or 0 then will be 1 day ago
    #### def getHourId(epoch=None) 
    
    is # hour from jan 1 2010
    #### def getLocalTimeHR() 
    
    Get the current local date and time in a human-readable form
    #### def getLocalTimeHRForFilesystem() 
    #### def getMinuteId(epoch=None) 
    
    is # min from jan 1 2010
    #### def getSecondsInHR(seconds) 
    #### def getTimeEpoch() 
    
    Get epoch timestamp (number of seconds passed since January 1, 1970)
    #### def getTimeEpochBin() 
    
    Get epoch timestamp (number of seconds passed since January 1, 1970)
