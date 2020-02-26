## Virtual enviroment
### Install and activate
In a terminal, from project folder:

```
python3 -m venv venv

source venv/bin/activate
```

## Config
### Make the krakenapi.py file executable.
You can use the "chmod 755" command (change mode). For example:

```
chmod 755 krakenapi.py
```

### API keys
Copy/paste your API public key from account management into file called "API_Public_Key".

Copy/paste your API private (secret) key into file called "API_Private_Key".

An API key is only needed if you plan to use the private API endpoints to access your Kraken account (such as balance inquiries, placing/cancelling orders, account history exports, etc).

## Usage: ./krakenapi.py method [parameters]
Examples: 

./krakenapi.py Time

./krakenapi.py OHLC pair=xbtusd interval=1440

./krakenapi.py Balance

./krakenapi.py OpenPositions
