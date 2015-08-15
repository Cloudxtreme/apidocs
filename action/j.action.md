## j.action

- /opt/jumpscale7/lib/JumpScale/baselib/actionsold/action/ActionController.py

### Methods

Manager controlling actions

#### def clean 
##### arguments

##### comments

Clean the list of running actions

#### def hasRunningActions 
##### arguments

##### comments

Check whether actions are currently running

@returns: Whether actions are runnin
@rtype: bool

#### def printOutput 
##### arguments

##### comments

#### def start 
##### arguments

- description
- errormessage
- resolutionmessage
- show = False
- messageLevel = False

##### comments

Start a new action

@param description: Description of the action
@type description: string
@param errormessage: Error message displayed to the user when the action
                     fails
@type errormessage: string
@param resolutionmessage: Resolution message displayed to the user when
                          the action fails
@type resolutionmessage: string

#### def startOutput 
##### arguments

##### comments

Enable j.console output. Format such that it is nicely shown between action start/stop.

#### def stop 
##### arguments

- failed = False

##### comments

Stop the currently running action

This will get the latest started action from the action stack and
display a result message.

@param failed: Whether the action failed
@type failed: bool

#### def stopOutput 
##### arguments

##### comments

Disable j.console output. Format such that it is nicely shown between action start/stop.

