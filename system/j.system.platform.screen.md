## j.system.platform.screen

- /opt/jumpscale7/lib/JumpScale/baselib/screen/Tmux.py
- Properties
    - screencmd

### Methods

#### def attachSession 
##### arguments

- sessionname
- windowname
- user
#### def createSession 
##### arguments

- sessionname
- screens
- user

##### comments

```
@param name is name of session
@screens is list with nr of screens required in session and their names (is [$screenname,...])

```

#### def createWindow 
##### arguments

- session
- name
- user
#### def executeInScreen 
##### arguments

- sessionname
- screenname
- cmd
- wait = 0
- cwd
- env
- user = 'root'
- tmuxuser

##### comments

```
@param sessionname Name of the tmux session
@type sessionname str
@param screenname Name of the window in the session
@type screenname str
@param cmd command to execute
@type cmd str
@param wait time to wait for output
@type wait int
@param cwd workingdir for command only in new screen see newscr
@type cwd str
@param env environment variables for cmd onlt in new screen see newscr
@type env dict

```

#### def getPid 
##### arguments

- session
- name
- user
#### def getSessions 
##### arguments

- user
#### def getWindows 
##### arguments

- session
- attemps = 5
- user
#### def killSession 
##### arguments

- sessionname
- user
#### def killSessions 
##### arguments

- user
#### def killWindow 
##### arguments

- session
- name
- user
#### def logWindow 
##### arguments

- session
- name
- filename
- user
#### def windowExists 
##### arguments

- session
- name
- user
