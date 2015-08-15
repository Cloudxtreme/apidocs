## j.base.time

- /opt/jumpscale7/lib/JumpScale/core/base/time/Time.py

### Methods

generic provider of time functions
lives at j.base.time

#### HRDatetoEpoch 
##### arguments

    - datestr
    - local = True

##### comments

convert string date to epoch
Date needs to be formatted as 16/06/1988

#### epoch2HRDate 
##### arguments

    - epoch
    - local = True

##### comments

#### epoch2HRDateTime 
##### arguments

    - epoch
    - local = True

##### comments

#### epoch2HRTime 
##### arguments

    - epoch
    - local = True

##### comments

#### fiveMinuteIdToEpoch 
##### arguments

    - fiveMinuteId

##### comments

#### formatTime 
##### arguments

    - epoch
    - formatstr = '%Y/%m/%d %H:%M:%S'
    - local = True

##### comments

Returns a formatted time string representing the current time

See http://docs.python.org/lib/module-time.html#l2h-2826 for an
overview of available formatting options.

@param format: Format string
@type format: string

@returns: Formatted current time
@rtype: string

#### get5MinuteId 
##### arguments

    - epoch

##### comments

is # 5 min from jan 1 2010

#### getDayId 
##### arguments

    - epoch

##### comments

is # day from jan 1 2010

#### getDeltaTime 
##### arguments

    - txt

##### comments

only supported now is -3m, -3d and -3h (ofcourse 3 can be any int)
and an int which would be just be returned
means 3 days ago 3 hours ago
if 0 or '' then is now

#### getEpochAgo 
##### arguments

    - txt

##### comments

only supported now is -3m, -3d and -3h  (ofcourse 3 can be any int)
and an int which would be just be returned
means 3 days ago 3 hours ago
if 0 or '' then is now

#### getEpochFuture 
##### arguments

    - txt

##### comments

only supported now is +3d and +3h  (ofcourse 3 can be any int)        
+3d means 3 days in future
and an int which would be just be returned
if txt==None or 0 then will be 1 day ago

#### getHourId 
##### arguments

    - epoch

##### comments

is # hour from jan 1 2010

#### getLocalTimeHR 
##### arguments

##### comments

Get the current local date and time in a human-readable form

#### getLocalTimeHRForFilesystem 
##### arguments

##### comments

#### getMinuteId 
##### arguments

    - epoch

##### comments

is # min from jan 1 2010

#### getSecondsInHR 
##### arguments

    - seconds

##### comments

#### getTimeEpoch 
##### arguments

##### comments

Get epoch timestamp (number of seconds passed since January 1, 1970)

#### getTimeEpochBin 
##### arguments

##### comments

Get epoch timestamp (number of seconds passed since January 1, 1970)

