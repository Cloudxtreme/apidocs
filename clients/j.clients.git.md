## j.clients.git

- /opt/jumpscale7/lib/JumpScale/baselib/git/GitFactory.py

    #### def find(account=None,name=None,interactive=False,returnGitClient=False) 
    
    walk over repo's known on system
    2 locations are checked
        ~/code
        /opt/code
    #### def get(basedir) 
    
    PLEASE USE SSH, see http://despiegk.gitbooks.io/jumpscale/content/Howto/how_to_use_git.html for more details
    #### def log(msg,category="",level=5) 
