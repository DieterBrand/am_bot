# am_bot
## Bot for [Too good to go](https://toogoodtogo.com) and [Foodsi](https://www.foodsi.pl/)
### Problem
This project helps me to no longer miss my favorite offers at [Too good to go](https://toogoodtogo.com) and [Foodsi](https://www.foodsi.pl/).

"Too good to go" and "Foodsi" are platforms, where stores can offer bags of leftover food, that they otherwise need to throw away. The stores save a little bit of money, we get goods, that already have a few quirks, but are still consumable. Most importantly, this reduces food waste and thereby is good for the planet. In my neighborhood, e.g. a supermarket offers fruits & vegetables and a bakery offer their leftover bread at the end of the day.

However, the Too good to go and Foodsi apps does often not notify me in time when my favorite goods are in stock. Since the offers are popular and limited, I regularly miss the time to click and collect the items. There are no settings for notifications in the apps.

### Solution
This application scrapes info from the Too good to go and Foodsi and sends me a notification via a Telegram bot as soon as some items in my area are available.
Here is a screenshot:
![Telegram Screenshot](/result_screenshot.jpeg "Telegram bot with notifications")


#### Tgtg API
There is a library wrapped around the API of the tgtg-app. You can find the library and a short documentation [here.](https://pypi.org/project/tgtg/)
##### How do I obtain credentails for tgtg?
Just run: 
```python3 watch_script.py <your_email>```

#### Telegram bot
I used Telegram as the service to notify me, because they are quite supportive for adding your own bots to the platform and provide a rich API. [This article](https://medium.com/@ManHay_Hong/how-to-create-a-telegram-bot-and-send-messages-with-python-4cf314d9fa3e) provides a quick introduction into sending Telegram messages with python.
