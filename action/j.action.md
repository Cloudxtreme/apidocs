## j.action

- /opt/jumpscale7/lib/JumpScale/baselib/actionsold/action/ActionController.py

Manager controlling actions

#### def clean() 

Clean the list of running actions

#### def hasRunningActions() 

Check whether actions are currently running

@returns: Whether actions are runnin
@rtype: bool

#### def printOutput() 

#### def start(description, errormessage=None, resolutionmessage=None, 

Start a new action

@param description: Description of the action
@type description: string
@param errormessage: Error message displayed to the user when the action
                     fails
@type errormessage: string
@param resolutionmessage: Resolution message displayed to the user when
                          the action fails
@type resolutionmessage: string

#### def startOutput() 

Enable j.console output. Format such that it is nicely shown between action start/stop.

#### def stop(failed=False) 

Stop the currently running action

This will get the latest started action from the action stack and
display a result message.

@param failed: Whether the action failed
@type failed: bool

#### def stopOutput() 

Disable j.console output. Format such that it is nicely shown between action start/stop.

