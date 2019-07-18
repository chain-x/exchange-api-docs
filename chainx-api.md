# ChainX API Document

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
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
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
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
    {
        "price": "",
        "volume": ""
    },
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


