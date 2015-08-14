## j.actions

- /opt/jumpscale7/lib/JumpScale/baselib/actions/action/ActionController.py

Manager controlling actions

### def reset(category=None) (l20)

### def hasRunningActions() (l76)

Check whether actions are currently running

@returns: Whether actions are runnin
@rtype: bool

### def start(description="", cmds="",action=None,actionRecover=None,actionArgs=\{\},category="unknown",name="unknown",\ (l43)

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

### def getActionNamesDone(action) (l28)

### def clean() (l69)

Clean the list of running actions

### def setActionNamesDone(action) (l35)

