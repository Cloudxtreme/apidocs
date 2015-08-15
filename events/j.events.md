## j.events

- /opt/jumpscale7/lib/JumpScale/core/errorhandling/EventHandler.py

#### bug_critical 
- arguments
    - msg
    - category = ''
    - jobid = 0
    - e
- comments
    will die
    @param e is python error object when doing except

#### bug_warning 
- arguments
    - msg
    - category = ''
    - e
- comments
    will die
    @param e is python error object when doing except

#### inputerror_critical 
- arguments
    - msg
    - category = ''
    - msgpub = ''
- comments
    will die

#### inputerror_warning 
- arguments
    - msg
    - category = ''
    - msgpub = ''
- comments
    will die

#### opserror 
- arguments
    - msg
    - category = ''
    - e
- comments
    will NOT die
    will make warning event is the same as opserror_warning
    @param e is python error object when doing except

#### opserror_critical 
- arguments
    - msg
    - category = ''
- comments
    will die

#### opserror_warning 
- arguments
    - msg
    - category = ''
    - e
- comments
    will NOT die
    will make warning event is the same as opserror_warning
    @param e is python error object when doing except

