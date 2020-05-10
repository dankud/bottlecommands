Retrieving data from a message.
=====================

```python
from vkbottle import Bot, Message

bot = Bot("token")

@bot.on.message_handler(text="Hello, my name is <name>", lower=True)
async def wrapper (ans: Message, name):
    await ans(f"Hello, {name}")
```
