## j.errorconditionhandler

- /opt/jumpscale7/lib/JumpScale/core/errorhandling/ErrorConditionHandler.py
- Properties
    - haltOnError
    - lastEco
    - redis
    - escalateToRedis
    - inException
    - lastAction

#### checkErrorIgnore 
- arguments
    - eco
- comments
    

#### escalateBugToDeveloper 
- arguments
    - errorConditionObject
    - tb
- comments
    

#### excepthook 
- arguments
    - ttype
    - pythonExceptionObject
    - tb
- comments
    every fatal error in jumpscale or by python itself will result in an exception
    in this function the exception is caught.
    This routine will create an errorobject & escalate to the infoserver
    @ttype : is the description of the error
    @tb : can be a python data object or a Event

#### getErrorConditionObject 
- arguments
    - ddict = \{\}
    - msg = ''
    - msgpub = ''
    - category = ''
    - level = 1
    - type = 'UNKNOWN'
    - tb
- comments
    @data is dict with fields of errorcondition obj
    returns only ErrorConditionObject which should be used in jumpscale to define an errorcondition (or potential error condition)

#### getErrorTraceKIS 
- arguments
    - tb
- comments
    

#### getFrames 
- arguments
    - tb
- comments
    

#### getLevelName 
- arguments
    - level
- comments
    

#### halt 
- arguments
    - msg
    - eco
- comments
    

#### lastActionClear 
- arguments
- comments
    clear last action so is not printed when error

#### lastActionSet 
- arguments
    - lastActionDescription
- comments
    will remember action you are doing, this will be added to error message if filled in

#### parsePythonErrorObject 
- arguments
    - pythonExceptionObject
    - ttype
    - tb
    - level = 1
    - message = ''
- comments
    how to use
    
    try:
        ##do something            
    except Exception,e:
        eco=j.errorconditionhandler.parsePythonErrorObject(e)
    
    eco is jumpscale internal format for an error 
    next step could be to process the error objecect (eco) e.g. by eco.process()
        
    @param pythonExceptionObject is errorobject thrown by python when there is an exception
    @param ttype : is the description of the error, can be None
    @param tb : can be a python data object for traceback, can be None
    
    @return a ErrorConditionObject object as used by jumpscale (should be the only type of object we send around)

#### processPythonExceptionObject 
- arguments
    - pythonExceptionObject
    - ttype
    - tb
    - level = 1
    - message = ''
    - sentry = True
- comments
    how to use
    
    try:
        ##do something            
    except Exception,e:
        j.errorconditionhandler.processpythonExceptionObject(e)
        
    @param pythonExceptionObject is errorobject thrown by python when there is an exception
    @param ttype : is the description of the error, can be None
    @param tb : can be a python data object for traceback, can be None
    
    @return [ecsource,ecid,ecguid]
    
    the errorcondition is then also processed e.g. send to local logserver and/or stored locally in errordb

#### raiseBug 
- arguments
    - message
    - category = ''
    - pythonExceptionObject
    - pythonTraceBack
    - msgpub = ''
    - die = True
    - tags = ''
    - level = 1
- comments
    use this to raise a bug in the code, this is the only time that a stacktrace will be asked for
    level will be Critical
    @param message is the error message which describes the bug
    @param msgpub is message we want to show to endcustomers (can include a solution)
    @param category is a dot notation to give category for the error condition
    @param pythonExceptionObject is the object as it comes from a try except statement
    
    try:
        ##do something            
    except Exception,e:
        j.errorconditionhandler.raiseBug("an error",category="exceptions.init",e)

#### raiseCritical 
- arguments
    - message
    - category = ''
    - pythonExceptionObject
    - pythonTraceBack
    - msgpub = ''
    - die = True
    - tags = ''
    - level = 1
- comments
    use this to raise a bug in the code, this is the only time that a stacktrace will be asked for
    level will be Critical
    @param message is the error message which describes the bug
    @param msgpub is message we want to show to endcustomers (can include a solution)
    @param category is a dot notation to give category for the error condition
    @param pythonExceptionObject is the object as it comes from a try except statement
    
    try:
        ##do something            
    except Exception,e:
        j.errorconditionhandler.raiseBug("an error",category="exceptions.init",e)

#### raiseInputError 
- arguments
    - message = ''
    - category = 'input'
    - msgpub = ''
    - die = True
    - backtrace = ''
    - tags = ''
- comments
    

#### raiseMonitoringError 
- arguments
    - message
    - category = ''
    - msgpub = ''
    - die = False
    - tags = ''
- comments
    

#### raiseOperationalCritical 
- arguments
    - message = ''
    - category = ''
    - msgpub = ''
    - die = True
    - tags = ''
    - eco
    - extra
- comments
    use this to raise an operational issue about the system
    @param message is message we want to use for operators
    @param msgpub is message we want to show to endcustomers (can include a solution)
    @param category is a dot notation to give category for the error condition

#### raiseOperationalWarning 
- arguments
    - message = ''
    - category = ''
    - msgpub = ''
    - tags = ''
    - eco
- comments
    

#### raisePerformanceError 
- arguments
    - message
    - category = ''
    - msgpub = ''
    - tags = ''
- comments
    

#### raiseRuntimeErrorWithEco 
- arguments
    - eco
    - tostdout = False
- comments
    

#### raiseWarning 
- arguments
    - message
    - category = ''
    - pythonExceptionObject
    - pythonTraceBack
    - msgpub = ''
    - tags = ''
- comments
    use this to raise a bug in the code, this is the only time that a stacktrace will be asked for
    @param message is the error message which describes the bug
    @param msgpub is message we want to show to endcustomers (can include a solution)
    @param category is a dot notation to give category for the error condition
    @param pythonExceptionObject is the object as it comes from a try except statement
    
    try:
        ##do something            
    except Exception,e:
        j.errorconditionhandler.raiseBug("an error",category="exceptions.init",e)

#### reRaiseECO 
- arguments
    - eco
- comments
    

#### setExceptHook 
- arguments
- comments
    

#### toolStripNonAsciFromText 
- arguments
    - text
- comments
    

