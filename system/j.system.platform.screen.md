## j.system.platform.screen

- /opt/jumpscale7/lib/JumpScale/baselib/screen/Tmux.py
- Properties
    - screencmd

#### def attachSession(sessionname, windowname=None,user=None) 

    

#### def createSession(sessionname,screens,user=None) 

    @param name is name of session
    @screens is list with nr of screens required in session and their names (is [$screenname,...])

#### def createWindow(session, name,user=None) 

    

#### def executeInScreen(sessionname,screenname,cmd,wait=0, cwd=None, env=None,user="root",tmuxuser=None) 

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

#### def getPid(session, name,user=None) 

    

#### def getSessions(user=None) 

    

#### def getWindows(session, attemps=5,user=None) 

    

#### def killSession(sessionname,user=None) 

    

#### def killSessions(user=None) 

    

#### def killWindow(session, name,user=None) 

    

#### def logWindow(session, name, filename,user=None) 

    

#### def windowExists(session, name,user=None) 

    

