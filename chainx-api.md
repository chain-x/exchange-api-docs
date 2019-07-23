# ChainX API Document
**API EndPoint URL: <https://api.chainx.kr/>**

## Account EndPoints
### [POST] Order

```
/api/v1/orders/
```

**Headers**

Key | Value
------------ | ------------
Content-Type | application/json
Authorization | Token

**Parameters:**

Name | Type | Mandatory | Description
------------ | ------------ | ------------ | ------------
trading_pair | STRING | YES | EX) "BTC-KRW", "ETH-KRW", "CXR-KRW"
side | STRING | YES | "SELL" OR "BUY"
volume | STRING | YES | "301232"
price | STRING | YES | "13"
order_type | STRING | YES | Default LIMIT;

**Response:**

```javascript
{
    "uuid": "",
    "trading_pair_name": "ETH-KRW",
    "side": "SELL",
    "volume": "13.00000000000000000000",
    "price": "301232.00000000000000000000",
    "volume_filled": "0.00000000000000000000",
    "volume_remaining": "3.00000000000000000000",
    "order_status": "PENDING",
    "order_type": "LIMIT",
    "created": "",
    "nickname": "",
    "trades": []
}
```

### [DELETE] Order Cancel

```
/api/v1/orders/{uuid}/
```

Key | Value
------------ | ------------
Content-Type | application/json
Authorization | Token

### [DELETE] Order Cancel All

```
/api/v1/orders/cancel_all/
```

Key | Value
------------ | ------------
Content-Type | application/json
Authorization | Token


## Market Data EndPoints
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



