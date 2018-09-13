AIQbot - Twitter Artiqox Tipping and Giving Platform.
Artiqox cryptocurrency tipping and giving platform for Twitter
Dependencies
apt-get install python3

apt-get install python3-pip

pip3 install requests
pip3 install tweepy
pip3 install subprocess
pip3 install json
pip3 install re
pip3 install 
pip3 install 

In order to run the tip-bot effectively, a Bitcoin-core based client is needed. For this git Artiqox Core is used , but any major alternate cryptocurrency client could easily be incorporated.

Setup
Download the git git clone https://github.com/znafca/aiqbot-twitter

Setup API tokens for tt account. and create secrets.py file with content:

consumer_key = 'xxx'
consumer_secret = 'xxx'

access_token = 'xxx'
access_secret = 'xxx'

Run the script python3 command.py

Bot tracks for tweets with specific pattern, some tweet examples:

- tweet with "bot_username @receivingUsername 20" will give @receivingUsername 20 AIQ
- tweet with "bot_username @receivingUsername 20 USD" will give @receivingUsername amount of AIQ that is equal to 20 USD
- tweet that is reply to another tweet (main) with "bot_username 20" will give author of the main tweet 20 AIQ
- tweet with "bot_username balance EUR" will give user balance in EUR
- tweet with "bot_username deposit" will give bot deposit address
- tweet with "bot_username withdraw aaaaaaa 20" will withdraw 20 AIQ to wallet aaaaaaa
- "bot_username help"

Setting up the bot as so still leaves the wallet unencrypted, so please go to extra measures to provide extra security. Make sure to have SSH encryption on whatever device/droplet you run it on.
Please fork the code, happy tipping!
