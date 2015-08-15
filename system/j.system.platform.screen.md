## j.system.platform.screen

- /opt/jumpscale7/lib/JumpScale/baselib/screen/Tmux.py
- Properties
    - screencmd

#### attachSession 
- arguments
    - sessionname
    - windowname
    - user
- comments
    

#### createSession 
- arguments
    - sessionname
    - screens
    - user
- comments
    @param name is name of session
    @screens is list with nr of screens required in session and their names (is [$screenname,...])

#### createWindow 
- arguments
    - session
    - name
    - user
- comments
    

#### executeInScreen 
- arguments
    - sessionname
    - screenname
    - cmd
    - wait = 0
    - cwd
    - env
    - user = 'root'
    - tmuxuser
- comments
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

#### getPid 
- arguments
    - session
    - name
    - user
- comments
    

#### getSessions 
- arguments
    - user
- comments
    

#### getWindows 
- arguments
    - session
    - attemps = 5
    - user
- comments
    

#### killSession 
- arguments
    - sessionname
    - user
- comments
    

#### killSessions 
- arguments
    - user
- comments
    

#### killWindow 
- arguments
    - session
    - name
    - user
- comments
    

#### logWindow 
- arguments
    - session
    - name
    - filename
    - user
- comments
    

#### windowExists 
- arguments
    - session
    - name
    - user
- comments
    

