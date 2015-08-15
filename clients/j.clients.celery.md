## j.clients.celery

- /opt/jumpscale7/lib/JumpScale/lib/celery/CeleryFactory.py
- Properties
    - app
    - actors

### Methods

#### def celeryClient 

##### arguments

- actorName
- url = 'redis://localhost:9999/0'
- actorsPath = 'actors'
- local = False

#### def celeryStart 

##### arguments

- url = 'redis://localhost:9999/0'
- concurrency = 4
- actorsPath = 'actors'

#### def flowerStart 

##### arguments

- url = 'redis://localhost:9999/0'

#### def getCodeClient 

##### arguments

- path
- actorName

#### def getCodeServer 

##### arguments

- path

