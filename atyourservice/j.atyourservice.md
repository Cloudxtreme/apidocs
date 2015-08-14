    #### def updateTemplatesRepo(repos=[]) 
    
    update the git repo that contains the service templates
    args:
        repos : list of dict of repos to update, if empty, all repos are updated
                \{
                    'url' : 'http://github.com/account/repo',
                    'branch' : 'master'
                \}
