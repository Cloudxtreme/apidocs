## j.atyourservice

- /opt/jumpscale7/lib/JumpScale/baselib/atyourservice/AtYourServiceFactory.py
- Properties
    - indocker
    - domains
    - hrd

### def getDomains() (l95)

### def findParents(service=None, name='', path='', limit=None) (l217)

### def get(domain="", name="", instance="", parent='', precise=False) (l266)

Return service indentifier by domain,name and instance
throw error if service is not found or if more than one service is found

### def getFromStr(representation, parent=None) (l359)

return a service instance from its representation 'domain      :name       :instance'

### def remove(domain="", name="", instance="", parent=None) (l258)

### def getId(domain, name, instance, parent=None) (l98)

### def findServices(domain="", name="", instance="", parent=None, precise=False) (l150)

FindServices looks for actual services that are created

### def updateTemplatesRepo(repos=[]) (l74)

update the git repo that contains the service templates
args:
    repos : list of dict of repos to update, if empty, all repos are updated
            {
                'url' : 'http://github.com/account/repo',
                'branch' : 'master'
            }

### def loadService(path, parent=None) (l289)

Load a service instance from files located at path.
path should point to a directory that contains these files:
    service.hrd
    actions.py

### def loadServicesInSQL() (l320)

walk over all services and load into sqllite

### def findTemplates(domain="", name="", parent=None) (l107)

### def new(domain="", name="", instance="main", path=None, parent=None, args={}) (l246)

will create a new service

### def findProducer(producercategory, instancename) (l241)

### def getActionsBaseClass() (l92)

