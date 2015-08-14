## j.system.platform.screen

- /opt/jumpscale7/lib/JumpScale/baselib/screen/Tmux.py
- Properties
    - screencmd

### def getSessions(user=None) (l101)

### def logWindow(session, name, filename,user=None) (l147)

### def createWindow(session, name,user=None) (l137)

### def windowExists(session, name,user=None) (l155)

### def getWindows(session, attemps=5,user=None) (l123)

### def killWindow(session, name,user=None) (l169)

### def executeInScreen(sessionname,screenname,cmd,wait=0, cwd=None, env=None,user="root",tmuxuser=None) (l39)

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

### def attachSession(sessionname, windowname=None,user=None) (l191)

### def killSessions(user=None) (l179)

### def getPid(session, name,user=None) (l110)

### def killSession(sessionname,user=None) (l185)

### def createSession(sessionname,screens,user=None) (l9)

@param name is name of session
@screens is list with nr of screens required in session and their names (is [$screenname,...])

