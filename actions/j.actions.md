## j.actions

- /opt/jumpscale7/lib/JumpScale/baselib/actions/action/ActionController.py

Manager controlling actions

#### clean 
- arguments
- comments
    Clean the list of running actions

#### getActionNamesDone 
- arguments
    - action
- comments
    

#### hasRunningActions 
- arguments
- comments
    Check whether actions are currently running
    
    @returns: Whether actions are runnin
    @rtype: bool

#### reset 
- arguments
    - category
- comments
    

#### setActionNamesDone 
- arguments
    - action
- comments
    

#### start 
- arguments
    - description = ''
    - cmds = ''
    - action
    - actionRecover
    - actionArgs = \{\}
    - category = 'unknown'
    - name = 'unknown'
    - errorMessage = ''
    - resolutionMessage = ''
    - loglevel = 1
    - die = True
    - stdOutput = True
    - errorOutput = True
    - retry = 1
    - serviceObj
- comments
    @param id is unique id which allows finding back of action
    @param description: Action description (what are we doing)
    @param errorMessage: message to give when error
    @param resolutionMessage: Action resolution message (how to resolve the action when error)
    @param loglevel: Message level
    @param action: python function to execute
    @param actionRecover: python function to execute when error
    @param actionArgs is dict with arguments
    @param cmds is list of commands to execute on os
    @param state : INIT,RUNNING,OK,ERROR

