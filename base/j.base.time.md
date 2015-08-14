## j.base.time

- /opt/jumpscale7/lib/JumpScale/core/base/time/Time.py

generic provider of time functions
lives at j.base.time

### def getEpochFuture(txt) (l155)

only supported now is +3d and +3h  (ofcourse 3 can be any int)        
+3d means 3 days in future
and an int which would be just be returned
if txt==None or 0 then will be 1 day ago

### def getSecondsInHR(seconds) (l31)

### def epoch2HRDate(epoch,local=True) (l86)

### def getLocalTimeHR() (l55)

Get the current local date and time in a human-readable form

### def getDayId(epoch=None) (l122)

is # day from jan 1 2010

### def fiveMinuteIdToEpoch(fiveMinuteId) (l113)

### def getEpochAgo(txt) (l144)

only supported now is -3m, -3d and -3h  (ofcourse 3 can be any int)
and an int which would be just be returned
means 3 days ago 3 hours ago
if 0 or '' then is now

### def epoch2HRDateTime(epoch,local=True) (l89)

### def getTimeEpochBin() (l48)

Get epoch timestamp (number of seconds passed since January 1, 1970)

### def getMinuteId(epoch=None) (l96)

is # min from jan 1 2010

### def HRDatetoEpoch(datestr,local=True) (l166)

convert string date to epoch
Date needs to be formatted as 16/06/1988

### def getHourId(epoch=None) (l107)

is # hour from jan 1 2010

### def getLocalTimeHRForFilesystem() (l61)

### def formatTime(epoch,formatstr='%Y/%m/%d %H%M%S',local=True) (l65)

Returns a formatted time string representing the current time

See http://docs.python.org/lib/module-time.html#l2h-2826 for an
overview of available formatting options.

@param format: Format string
@type format: string

@returns: Formatted current time
@rtype: string

### def getDeltaTime(txt) (l129)

only supported now is -3m, -3d and -3h (ofcourse 3 can be any int)
and an int which would be just be returned
means 3 days ago 3 hours ago
if 0 or '' then is now

### def epoch2HRTime(epoch,local=True) (l92)

### def get5MinuteId(epoch=None) (l116)

is # 5 min from jan 1 2010

### def getTimeEpoch() (l20)

Get epoch timestamp (number of seconds passed since January 1, 1970)

