# crypto-trading-bot
## What is this?
- crypto market trading bot
- auto trading by the rule : buy low sell high
## How to run it?
- install nodejs
- install packages
- input your secret key, access key
```javascript
const access_key = 'YOUR ACCESS KEY';
const secret_key = 'YOUR SECRET KEY';
```
- input your initial capital
```javascript
let Initial_KRW_remain = 420000; // YOUR INITIAL CAPITAL : direct recog.
```
- input market code
```javascript
const tick_options = {
  method: 'GET',
	url: 'https://api.upbit.com/v1/ticker',
	qs: { markets: 'KRW-XRP'},
};
```
```javascript
const bid_body = {
	market: 'KRW-XRP',
	side: 'bid',
	volume: JSON.stringify(volume_bidding),
	price: JSON.stringify(Bought_price),
	ord_type: 'limit',
};

const ask_body = {
	market: 'KRW-XRP',
	side: 'ask',
	volume: JSON.stringify(Holding_vol),
	price: null,
	ord_type: 'market',
}
```
- run it
```javascript
node real_trade.js
```
## you wanna simulate?
```javascript
node trade_virtual.js
```
## Contribute
- welcome
***
## Problems and ideas to solve
- make package.json
- slump trending
  - intermarket
    - testing intermarket virtual trade in multi process
    - testing ML(using tensorflow) and read data
- soaring trending
  - change cnt value
- trash readme.md
  - relax
## Conclusion
- no solution.
- bye bye
