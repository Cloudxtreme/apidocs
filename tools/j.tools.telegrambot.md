## j.tools.telegrambot

- /opt/jumpscale7/lib/JumpScale/lib/telegram/TelegramFactory.py

### Methods

#### def demo 

##### arguments

##### comments

```
tg=self.get()
tg.addDemoHandler()
tg.start()

```

#### def demoMS1 

##### arguments

##### comments

```
instructions how to load a handler

tg=j.tools.telegrambot.get()
from handlers.DemoHandlerMS1 import *
handler = DemoHandlerMS1()
tg.api.add_handler(handler)
tg.start()

```

#### def get 

##### arguments

- telegramkey = ''

##### comments

```
@param telegramkey eg. 112456445:AAFgQVEWPGztQc1S8NW0NXY8rqQLDPx0knM
if not filled in will try to get from env variable: telegram
set as follows: export telegram=1124...

```

