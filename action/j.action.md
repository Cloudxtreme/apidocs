## j.action

- /opt/jumpscale7/lib/JumpScale/baselib/actionsold/action/ActionController.py

Manager controlling actions

### def startOutput() (l286)

Enable j.console output. Format such that it is nicely shown between action start/stop.

### def printOutput() (l277)

### def stop(failed=False) (l222)

Stop the currently running action

This will get the latest started action from the action stack and
display a result message.

@param failed: Whether the action failed
@type failed: bool

### def hasRunningActions() (l269)

Check whether actions are currently running

@returns: Whether actions are runnin
@rtype: bool

### def start(description, errormessage=None, resolutionmessage=None, (l185)

Start a new action

@param description: Description of the action
@type description: string
@param errormessage: Error message displayed to the user when the action
                     fails
@type errormessage: string
@param resolutionmessage: Resolution message displayed to the user when
                          the action fails
@type resolutionmessage: string

### def clean() (l262)

Clean the list of running actions

### def stopOutput() (l302)

Disable j.console output. Format such that it is nicely shown between action start/stop.

