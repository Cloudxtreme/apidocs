## j.clients.celery

- /opt/jumpscale7/lib/JumpScale/lib/celery/CeleryFactory.py
- Properties
    - app
    - actors

### Methods

#### celeryClient 
##### arguments

    - actorName
    - url = 'redis://localhost:9999/0'
    - actorsPath = 'actors'
    - local = False

##### comments

#### celeryStart 
##### arguments

    - url = 'redis://localhost:9999/0'
    - concurrency = 4
    - actorsPath = 'actors'

##### comments

#### flowerStart 
##### arguments

    - url = 'redis://localhost:9999/0'

##### comments

#### getCodeClient 
##### arguments

    - path
    - actorName

##### comments

#### getCodeServer 
##### arguments

    - path

##### comments

