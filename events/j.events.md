## j.events

- /opt/jumpscale7/lib/JumpScale/core/errorhandling/EventHandler.py

#### def bug_critical(msg,category="",jobid=0,e=None) 

will die
@param e is python error object when doing except

#### def bug_warning(msg,category="",e=None) 

will die
@param e is python error object when doing except

#### def inputerror_critical(msg,category="",msgpub="") 

will die

#### def inputerror_warning(msg,category="",msgpub="") 

will die

#### def opserror(msg,category="",e=None) 

will NOT die
will make warning event is the same as opserror_warning
@param e is python error object when doing except

#### def opserror_critical(msg,category="") 

will die

#### def opserror(msg,category="",e=None) 

will NOT die
will make warning event is the same as opserror_warning
@param e is python error object when doing except

