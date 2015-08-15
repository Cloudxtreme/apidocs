## j.atyourservice

- /opt/jumpscale7/lib/JumpScale/baselib/atyourservice/AtYourServiceFactory.py
- Properties
    - indocker
    - domains
    - hrd

### Methods

#### def findParents 
##### arguments

- service
- name = ''
- path = ''
- limit

##### comments

#### def findProducer 
##### arguments

- producercategory
- instancename

##### comments

#### def findServices 
##### arguments

- domain = ''
- name = ''
- instance = ''
- parent
- precise = False

##### comments

FindServices looks for actual services that are created

#### def findTemplates 
##### arguments

- domain = ''
- name = ''
- parent

##### comments

#### def get 
##### arguments

- domain = ''
- name = ''
- instance = ''
- parent = ''
- precise = False

##### comments

Return service indentifier by domain,name and instance
throw error if service is not found or if more than one service is found

#### def getActionsBaseClass 
##### arguments

##### comments

#### def getDomains 
##### arguments

##### comments

#### def getFromStr 
##### arguments

- representation
- parent

##### comments

return a service instance from its representation 'domain      :name       :instance'

#### def getId 
##### arguments

- domain
- name
- instance
- parent

##### comments

#### def loadService 
##### arguments

- path
- parent

##### comments

Load a service instance from files located at path.
path should point to a directory that contains these files:
    service.hrd
    actions.py

#### def loadServicesInSQL 
##### arguments

##### comments

walk over all services and load into sqllite

#### def new 
##### arguments

- domain = ''
- name = ''
- instance = 'main'
- path
- parent
- args = \{\}

##### comments

will create a new service

#### def remove 
##### arguments

- domain = ''
- name = ''
- instance = ''
- parent

##### comments

#### def updateTemplatesRepo 
##### arguments

- repos = []

##### comments

update the git repo that contains the service templates
args:
    repos : list of dict of repos to update, if empty, all repos are updated
            \{
                'url' : 'http://github.com/account/repo',
                'branch' : 'master'
            \}

