## j.clients.gitlab

- /opt/jumpscale7/lib/JumpScale/baselib/gitlab/GitlabFactory.py
- Properties
    - connections

Gitlab client enables administrators and developers leveraging Gitlab services through JumpScale

#### def get(gitlaburl="",login="",passwd="",instance="main") 

    example for gitlaburl
        https://despiegk:dddd@git.aydo.com
    can also be without login:passwd
        e.g. https://git.aydo.com and specify login/passwd
    
    if gitlaburl is empty then 
        hrd is used as follows:
        hrd=j.application.getAppInstanceHRD("gitlab_client",instance)
        gitlaburl=hrd.get("gitlab.client.url")
        login=hrd.get("gitlab.client.login")
        passwd=hrd.get("gitlab.client.passwd")

#### def getAccountnameReponameFromUrl(url) 

    

#### def log(msg,category="",level=5) 

    

