# config.py

keys = {
    'евро': 'EUR',
    'доллар': 'ЮэСДэ',  # Неправильное обозначение валюты (USD).
    'рубль': 'RUB',
}

#################################################################

# extensions.py

import json
import requests
from config import *    # Не дописана строка (keys)

 r = requests.get(
            f'https://min-api.cryptocompare.com/data/price?fsym={base_ticker}&tsyms={quote_ticker}')    # quote_ticker должен быть первым, а base_ticker вторым.
        total_base = float(json.loads(r.content)[keys[quote]])                                          # total_base берёт данные от keys[base].
        return total_base
