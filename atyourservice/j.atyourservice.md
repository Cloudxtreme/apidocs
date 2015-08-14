## j.atyourservice

- /opt/jumpscale7/lib/JumpScale/baselib/atyourservice/AtYourServiceFactory.py
- Properties
    - indocker
    - domains
    - hrd

#### def findParents(service=None, name='', path='', limit=None) 

    

#### def findProducer(producercategory, instancename) 

    

#### def findServices(domain="", name="", instance="", parent=None, precise=False) 

    FindServices looks for actual services that are created

#### def findTemplates(domain="", name="", parent=None) 

    

#### def get(domain="", name="", instance="", parent='', precise=False) 

    Return service indentifier by domain,name and instance
    throw error if service is not found or if more than one service is found

#### def getActionsBaseClass() 

    

#### def getDomains() 

    

#### def getFromStr(representation, parent=None) 

    return a service instance from its representation 'domain      :name       :instance'

#### def getId(domain, name, instance, parent=None) 

    

#### def loadService(path, parent=None) 

    Load a service instance from files located at path.
    path should point to a directory that contains these files:
        service.hrd
        actions.py

#### def loadServicesInSQL() 

    walk over all services and load into sqllite

#### def new(domain="", name="", instance="main", path=None, parent=None, args=\{\}) 

    will create a new service

#### def remove(domain="", name="", instance="", parent=None) 

    

#### def updateTemplatesRepo(repos=[]) 

    update the git repo that contains the service templates
    args:
        repos : list of dict of repos to update, if empty, all repos are updated
                \{
                    'url' : 'http://github.com/account/repo',
                    'branch' : 'master'
                \}

