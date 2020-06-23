![Executium API Version 2](https://i.imgur.com/nn0w8Eo.jpg)

# Executium API Version 2 Documentation
Executium version 2 is currently in private beta mode as we look to launch our new version of executium which has hundreds of new options and an extensive API which can connect with your business. 

## All Official Documentation for Executium
* Announcements regarding changes, upgrades, important exchange information, fixes, etc. to the API and Trading System will be reported here: **UPDATING-URL**
* Endpoints, parameters, payloads, etc. outlined in the documents in this repo are considered **official releases** and **supported by executium**.
* The use of any other endpoints, parameters, or payloads, etc. not outlined in this repo and the documents within are **not supported** and you **use them at your own risk and with no guarantees of functionality**.


Name | Description
------------ | ------------
[rest-api.md](./rest-api.md) | Detailed information on the Executium V2 Rest API (/api/v2)
[errors.md](./errors.md) | Details and descriptions of error messages from the Rest API
[symbols-supported.md](./symbols-supported.md) | Information related to the current supported symbols by executium.
[exchanges-supported.md](./exchanges-supported.md) | Information related to the current supported exchanges by executium.

## Supported Exchanges in Version 2
A table of supported exchanges in executium for version 2. The following table is the status as of 23rd June 2020.

Exchange | Executium Code |Active | Symbols Count
------------ | ------------ | ------------ | ------------
Binance|binance|Yes|583
Bitfinex|bitfinex|Yes|294
Bitflyer|bitflyer|Yes|10
Bithumb|bithumb|Yes|109
Bitmart|bitmart|Yes|5
Bitmax|bitmax|Yes|202
Bitmex|bitmex|Yes|13
Bitstamp|bitstamp|Yes|32
Bittrex|bittrex|Yes|415
Coinbase|coinbase|Yes|169
Coinbasepro|coinbasepro|Yes|67
Coincheck|coincheck|Yes|1
Deribit|deribit|Yes|8
Ftx|ftx|Yes|374
Gateio|gateio|Yes|469
Huobipro|huobipro|Yes|558
Indodax|indodax|Yes|68
Itbit|itbit|Yes|6
Kraken|kraken|Yes|155
Kucoin|kucoin|Yes|437
Liquid|liquid|Yes|176
Okex|okex|Yes|365
Poloniex|poloniex|Yes|149
Upbit|upbit|Yes|259


## Supported Symbols in Version 2
We have increased our symbols and exchange support with version 2, as of the 22nd June 2020 (https://executium.com/symbols-exchanges-marketspreads/). 

Version | Exchanges | Markets | Market Spreads | Permutation 
------------ | ------------ | ------------  | ------------   | ------------
Version 2|24|4,924|12,120,426 | 24,240,852
Version 1|12|140|869 | 869

### Quote to Quote Permutation

Quote | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
BTC|1481|2,193,361|Binance, Bitfinex, Bitflyer, Bitmart, Bitmax, Bittrex, Coinbasepro, Ftx, Kucoin, Liquid, Okex, Poloniex, Upbit
ETH|747|558,009|Binance, Bitfinex, Bitmax, Bittrex, Coinbasepro, Kucoin, Liquid, Okex, Poloniex
USDT|1007|1,014,049|Binance, Bitmart, Bitmax, Bittrex, Ftx, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
BNB|80|6,400|Binance, Kucoin
TUSD|22|484|Binance, Kucoin
PAX|25|625|Binance, Bitmart, Bitmax, Kucoin, Poloniex
USDC|69|4,761|Binance, Bitmart, Bitmax, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
TRX|19|361|Binance, Kucoin, Poloniex
BUSD|38|1,444|Binance
NGN|4|16|Binance, Coinbase
RUB|7|49|Binance, Coinbase
TRY|7|49|Binance, Coinbase
EUR|47|2,209|Binance, Bitfinex, Bitflyer, Bittrex, Coinbase, Coinbasepro, Itbit, Liquid
ZAR|6|36|Binance, Coinbase
BKRW|3|9|Binance
IDRT|5|25|Binance, Liquid
USD|529|279,841|Bitfinex, Bitflyer, Bittrex, Coinbase, Coinbasepro, Deribit, Ftx, Itbit, Liquid
JPY|20|400|Bitfinex, Bitflyer, Coinbase, Liquid
GBP|21|441|Bitfinex, Coinbase, Coinbasepro
EOS|3|9|Bitfinex
DAI|14|196|Bitfinex, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
UST|19|361|Bitfinex
CNHT|3|9|Bitfinex
USTF0|4|16|Bitfinex
KRW|199|39,601|Bithumb, Coinbase, Upbit
XBT|7|49|Bitmex
CUSTOM1|6|36|Bitmex
AUD|4|16|Coinbase, Liquid
BRL|2|4|Coinbase, Ftx
CHF|6|36|Coinbase, Kraken
HKD|3|9|Coinbase, Liquid
IDR|58|3,364|Coinbase
PHP|2|4|Coinbase, Liquid
SGD|8|64|Coinbase, Itbit, Liquid
XETH|23|529|Kraken
ZEUR|33|1,089|Kraken
ZUSD|35|1,225|Kraken
XXBT|29|841|Kraken
ZGBP|7|49|Kraken
ZCAD|6|36|Kraken
ZJPY|6|36|Kraken
NEO|7|49|Kucoin
KCS|7|49|Kucoin
QASH|18|324|Liquid
USDK|30|900|Okex
OKB|13|169|Okex
USDJ|3|9|Poloniex

We are adding and updating symbols supported by executium daily, the list for [Symbols Supported](./symbols-supported.md) can be monitored. We intend to update this support list weekly with version 2, and for a real-time look at support you can access via the api endpoint `system/symbols` for a full list of support symbols, or keep up to date in real-time via the executium website.
