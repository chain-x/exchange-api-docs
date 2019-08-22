# ChainX API Document
**API EndPoint URL: <https://api.chainx.kr/>**

## Asset Status List
### [GET] Asset

```
/api/v1.0/trading_pairs/coinmarketcap_assets/
```

**Response:**

```javascript
{
    "key": {
    	"lastUpdateTimestamp": "2019-06-14T15:30:10.000Z",
    	"name": "Ethereum"
    }
}
```


## Ticker Summary
### [GET] Ticker

```
/api/v1.0/trading_pairs/coinmarketcap_ticker/
```

**Response:**

```javascript
{
    "key": {
    	"lastUpdateTimestamp": "2019-06-14T15:30:10.000Z",
    	"tradingPairs": "ETH_KRW",
	"LastPrice": "0.01",
	"lowestAsk": "0.01",
	"highestBid": "0.01",
	"baseVolume24h": "10000",
	"quoteVolume24h": "100",
	"tradesEnabled": "True"
    }
}
```


## Recent Trades
### [GET] Trades

```
/api/v1.0/tradess/<Market Pair>/
```

**Response:**

```javascript
{
    "Market Pair": {
    	"tradeID": "23125",
    	"price": "0.01",
	"baseVolume": "50",
	"quoteVolume": "1.2",
	"time": "2019-06-14T15:30:10.000Z",
	"isBuyerMaker": "True"
    }
}
```


## Orderbook
### [GET] Orderbook

```
/api/v1.0/trading_pairs/<Market Pair>/
```

**Response:**

```javascript
{
    "lastUpdateTimestamp": "2019-06-14T15:30:10.000Z",
    "bids": {
    	"PRICE": "4",
	"QTY": "3"
    },
    "asks": {
    	"PRICE": "4",
	"QTY": "3"
    }
}
```
