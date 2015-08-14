## j.actions

- /opt/jumpscale7/lib/JumpScale/baselib/actions/action/ActionController.py

Manager controlling actions

#### def clean() 

    Clean the list of running actions

#### def getActionNamesDone(action) 

    

#### def hasRunningActions() 

    Check whether actions are currently running
    
    @returns: Whether actions are runnin
    @rtype: bool

#### def reset(category=None) 

    

#### def setActionNamesDone(action) 

    

#### def start(description="", cmds="",action=None,actionRecover=None,actionArgs=\{\},category="unknown",name="unknown",\ 

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

