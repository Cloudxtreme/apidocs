## j.events

- /opt/jumpscale7/lib/JumpScale/core/errorhandling/EventHandler.py

### def opserror(msg,category="",e=None) (l39)

will NOT die
will make warning event is the same as opserror_warning
@param e is python error object when doing except

### def bug_critical(msg,category="",jobid=0,e=None) (l5)

will die
@param e is python error object when doing except

### def opserror(msg,category="",e=None) (l39)

will NOT die
will make warning event is the same as opserror_warning
@param e is python error object when doing except

### def bug_warning(msg,category="",e=None) (l20)

will die
@param e is python error object when doing except

### def opserror_critical(msg,category="") (l30)

will die

### def inputerror_critical(msg,category="",msgpub="") (l50)

will die

### def inputerror_warning(msg,category="",msgpub="") (l56)

will die

