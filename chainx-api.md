# ChainX API Document
**API EndPoint URL: <https://api.chainx.kr/>**


## Market Data EndPoint

### [GET] Order Book
```
/api/v1/trading_pairs/orderbook
```

**Parameters:**

Name | Type | Mandatory | Description
------------ | ------------ | ------------ | ------------
trading_pair_name | STRING | YES | EX) "BTC-KRW", "ETH-KRW", "CXR-KRW"

**Response:**
```javascript
{
  "buys": [
    {
	"price": "",
	"volume": ""
    },
    {
        "price": "",
        "volume": ""
    }
  ],
  "sells": [
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    }
  ]

}
```

### [GET] Recent Trades List
```
/api/v1/trades/last_trade
```

**Parameters:**

Name | Type | Mandatory | Description
------------ | ------------ | ------------ | ------------
trading_pair_name | STRING | YES | EX) "BTC-KRW", "ETH-KRW", "CXR-KRW"
limit | INT | NO | Default 500; max 1000

**Response:**
```javascript
[
  {
    "id": 23131,
    "price": "",
    "qty": "",
    "side": "SELL",
    "created": "",
  } 
]
```



