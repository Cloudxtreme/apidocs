## j.tools.telegrambot

- /opt/jumpscale7/lib/JumpScale/lib/telegram/TelegramFactory.py

### def demo() (l22)

tg=self.get()
tg.addDemoHandler()
tg.start()

### def get(telegramkey="") (l8)

@param telegramkey eg. 112456445:AAFgQVEWPGztQc1S8NW0NXY8rqQLDPx0knM
if not filled in will try to get from env variable: telegram
set as follows: export telegram=1124...

### def demoMS1() (l32)

instructions how to load a handler

tg=j.tools.telegrambot.get()
from handlers.DemoHandlerMS1 import *
handler = DemoHandlerMS1()
tg.api.add_handler(handler)
tg.start()

