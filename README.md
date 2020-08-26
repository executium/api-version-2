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
The following table is the status as of 26th August 2020.

Exchange | Executium Code |Active | Symbols Count
------------ | ------------ | ------------ | ------------
Binance|binance|Yes|706
Binancefutures|binancefutures|Yes|41
Bitfinex|bitfinex|Yes|292
Bitflyer|bitflyer|Yes|10
Bithumb|bithumb|Yes|106
Bitmart|bitmart|Yes|5
Bitmex|bitmex|Yes|15
Bitstamp|bitstamp|Yes|32
Bittrex|bittrex|Yes|506
Bybit|bybit|Yes|5
Coinbase|coinbase|Yes|169
Coinbasepro|coinbasepro|Yes|82
Coincheck|coincheck|Yes|1
Deribit|deribit|Yes|8
Ftx|ftx|Yes|372
Gateio|gateio|Yes|500
Hbdm|hbdm|Yes|44
Huobipro|huobipro|Yes|624
Indodax|indodax|Yes|68
Itbit|itbit|Yes|6
Kraken|kraken|Yes|155
Krakenfutures|krakenfutures|Yes|19
Kucoin|kucoin|Yes|467
Liquid|liquid|Yes|158
Okex|okex|Yes|408
Okexfutures|okexfutures|Yes|408
Okexswap|okexswap|Yes|408
Poloniex|poloniex|Yes|228
Upbit|upbit|Yes|268
Zb|zb|Yes|158

## Supported Symbols in Version 2
We have increased our symbols and exchange support with version 2, as of the 26th August 2020 (https://executium.com/symbols-exchanges-marketspreads/). 

Version | Exchanges | Markets | Market Spreads | Permutation 
------------ | ------------ | ------------  | ------------   | ------------
Version 2|25|6,269|19,647,046|39,294,092
Version 1|12|138|871 | 871

### Quote to Quote Permutation

Quote | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
BTC|1782|3,175,524|Binance, Bitfinex, Bitflyer, Bitmart, Bittrex, Coinbasepro, Ftx, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ETH|864|746,496|Binance, Bitfinex, Bittrex, Coinbasepro, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex
USDT|1548|2,396,304|Binance, Binancefutures, Bitmart, Bittrex, Bybit, Ftx, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
BNB|97|9,409|Binance, Poloniex
TUSD|17|289|Binance, Kucoin
PAX|18|324|Binance, Bitmart, Kucoin, Poloniex
USDC|87|7,569|Binance, Bitmart, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex
TRX|28|784|Binance, Kucoin, Poloniex
BUSD|83|6,889|Binance, Poloniex
NGN|4|16|Binance, Coinbase
RUB|7|49|Binance, Coinbase
TRY|7|49|Binance, Coinbase
EUR|56|3,136|Binance, Bitfinex, Bitflyer, Bittrex, Coinbase, Coinbasepro, Itbit, Liquid
ZAR|6|36|Binance, Coinbase
BKRW|7|49|Binance
IDRT|5|25|Binance, Liquid
GBP|31|961|Binance, Bitfinex, Coinbase, Coinbasepro
UAH|3|9|Binance, Coinbase
BIDR|5|25|Binance
AUD|8|64|Binance, Coinbase, Liquid
DAI|22|484|Binance, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex
USD|565|319,225|Bitfinex, Bitflyer, Bittrex, Bybit, Coinbase, Coinbasepro, Deribit, Ftx, Itbit, Liquid
JPY|19|361|Bitfinex, Bitflyer, Coinbase, Liquid
EOS|2|4|Bitfinex
UST|23|529|Bitfinex
CNHT|3|9|Bitfinex
USTF0|5|25|Bitfinex
KRW|205|42,025|Bithumb, Coinbase, Upbit
XBT|7|49|Bitmex
CUSTOM1|8|64|Bitmex
BRL|2|4|Coinbase, Ftx
CHF|6|36|Coinbase, Kraken
HKD|3|9|Coinbase, Liquid
IDR|58|3,364|Coinbase
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
QASH|13|169|Liquid
USDK|93|8,649|Okex, Okexfutures, Okexswap
OKB|36|1,296|Okex, Okexfutures, Okexswap
USDJ|3|9|Poloniex


### Base to Base Permutation

Base | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
ETH|112|12,544|Binance, Binancefutures, Bitfinex, Bitflyer, Bithumb, Bitmart, Bitmex, Bittrex, Bybit, Coinbasepro, Deribit, Ftx, Hbdm, Itbit, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
LTC|75|5,625|Binance, Binancefutures, Bitfinex, Bithumb, Bitmex, Bittrex, Coinbasepro, Ftx, Hbdm, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
BNB|30|900|Binance, Binancefutures, Ftx, Kucoin, Poloniex
NEO|44|1,936|Binance, Binancefutures, Bitfinex, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
QTUM|37|1,369|Binance, Binancefutures, Bithumb, Bittrex, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
EOS|76|5,776|Binance, Binancefutures, Bitfinex, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hbdm, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
SNT|24|576|Binance, Bitfinex, Bithumb, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
BTC|278|77,284|Binance, Binancefutures, Bitfinex, Bitflyer, Bithumb, Bitmart, Bittrex, Bybit, Coinbase, Coinbasepro, Deribit, Ftx, Hbdm, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
MCO|20|400|Binance, Bithumb, Bittrex, Okex, Okexfutures, Okexswap
LRC|23|529|Binance, Bitfinex, Bithumb, Bittrex, Okex, Okexfutures, Okexswap, Poloniex, Upbit
OMG|44|1,936|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ZRX|41|1,681|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
KNC|30|900|Binance, Binancefutures, Bitfinex, Bithumb, Coinbasepro, Ftx, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
IOTA|26|676|Binance, Binancefutures, Bittrex, Okex, Okexfutures, Okexswap, Upbit
LINK|56|3,136|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Coinbasepro, Ftx, Hbdm, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ETC|62|3,844|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Coinbasepro, Ftx, Hbdm, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ZEC|40|1,600|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
DASH|44|1,936|Binance, Binancefutures, Bithumb, Bittrex, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex
TRX|72|5,184|Binance, Binancefutures, Bitfinex, Bithumb, Bitmex, Bittrex, Ftx, Hbdm, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
XRP|91|8,281|Binance, Binancefutures, Bitfinex, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hbdm, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
XMR|33|1,089|Binance, Binancefutures, Bitfinex, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
BAT|41|1,681|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kraken, Okex, Okexfutures, Okexswap, Poloniex, Upbit
LSK|24|576|Binance, Bittrex, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
MANA|28|784|Binance, Bittrex, Coinbasepro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ADA|52|2,704|Binance, Binancefutures, Bitfinex, Bithumb, Bitmex, Bittrex, Ftx, Hbdm, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Upbit
XLM|47|2,209|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kucoin, Okex, Okexfutures, Okexswap, Upbit
LEND|21|441|Binance, Binancefutures, Okex, Okexfutures, Okexswap, Poloniex
WAVES|32|1,024|Binance, Binancefutures, Bithumb, Bittrex, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Upbit
ICX|24|576|Binance, Bithumb, Bittrex, Kraken, Okex, Okexfutures, Okexswap, Upbit
ELF|23|529|Binance, Bitfinex, Bithumb, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Upbit
IOST|24|576|Binance, Binancefutures, Bithumb, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Upbit
NANO|25|625|Binance, Kraken, Kucoin, Okex, Okexfutures, Okexswap
ZIL|27|729|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Upbit
ONT|27|729|Binance, Binancefutures, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Upbit
XEM|25|625|Binance, Bithumb, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
GNT|25|625|Binance, Bitfinex, Bithumb, Bittrex, Coinbasepro, Okex, Okexfutures, Okexswap, Poloniex, Upbit
CVC|24|576|Binance, Bittrex, Coinbasepro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
THETA|20|400|Binance, Binancefutures, Bithumb, Ftx, Okex, Okexfutures, Okexswap, Upbit
SC|31|961|Binance, Bittrex, Kraken, Okex, Okexfutures, Okexswap, Poloniex, Upbit
VET|23|529|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Ftx, Kucoin, Upbit
HC|22|484|Binance, Kucoin, Okex, Okexfutures, Okexswap
PAX|20|400|Binance, Bitfinex, Bittrex, Okex, Okexfutures, Okexswap, Poloniex, Upbit
RVN|20|400|Binance, Bittrex, Okex, Okexfutures, Okexswap, Upbit
DCR|23|529|Binance, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
BCH|65|4,225|Binance, Binancefutures, Bitflyer, Bithumb, Bitmex, Bittrex, Coinbasepro, Ftx, Hbdm, Kraken, Liquid, Okex, Okexfutures, Okexswap, Upbit
BTT|37|1,369|Binance, Bitfinex, Bithumb, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ATOM|41|1,681|Binance, Binancefutures, Bittrex, Coinbasepro, Ftx, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ALGO|38|1,444|Binance, Binancefutures, Bithumb, Bittrex, Coinbasepro, Ftx, Kraken, Kucoin, Okex, Okexfutures, Okexswap
DOGE|31|961|Binance, Binancefutures, Bittrex, Ftx, Okex, Okexfutures, Okexswap, Poloniex, Upbit
XTZ|43|1,849|Binance, Binancefutures, Bitfinex, Bithumb, Bittrex, Coinbasepro, Ftx, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
HBAR|22|484|Binance, Bittrex, Liquid, Okex, Okexfutures, Okexswap, Upbit
USDT|31|961|Binance, Bittrex, Ftx, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
MDT|20|400|Binance, Bittrex, Okex, Okexfutures, Okexswap, Poloniex
DGB|23|529|Binance, Bitfinex, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Upbit
COMP|29|841|Binance, Binancefutures, Bittrex, Coinbasepro, Ftx, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
SNX|21|441|Binance, Binancefutures, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
MKR|35|1,225|Binance, Binancefutures, Bitfinex, Coinbasepro, Ftx, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
BAL|20|400|Binance, Ftx, Okex, Okexfutures, Okexswap, Poloniex
ANT|20|400|Binance, Bitfinex, Bittrex, Okex, Okexfutures, Okexswap, Upbit
DOT|31|961|Binance, Binancefutures, Bitfinex, Bittrex, Ftx, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
BSV|31|961|Bitfinex, Bithumb, Bittrex, Ftx, Hbdm, Okex, Okexfutures, Okexswap, Upbit
LEO|22|484|Bitfinex, Ftx, Okex, Okexfutures, Okexswap
OKB|21|441|Bitfinex, Ftx, Okex, Okexfutures, Okexswap
CRO|27|729|Bithumb, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Upbit
BTM|20|400|Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Upbit


### Pairing Permutation (Exact symbol match)

Base | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
ETHBTC|20|400|Binance, Bitfinex, Bitflyer, Bitmart, Bitstamp, Bittrex, Coinbasepro, Ftx, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
LTCBTC|17|289|Binance, Bitfinex, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
BNBBTC|2|4|Binance, Kucoin
NEOBTC|11|121|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Zb
QTUMETH|8|64|Binance, Bittrex, Gateio, Huobipro, Kraken, Okex, Okexfutures, Okexswap
EOSETH|11|121|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
SNTETH|4|16|Binance, Bittrex, Gateio, Kucoin
BNTETH|3|9|Binance, Bittrex, Gateio
GASBTC|8|64|Binance, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
BTCUSDT|18|324|Binance, Binancefutures, Bitfinex, Bitmart, Bittrex, Bybit, Ftx, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
ETHUSDT|17|289|Binance, Binancefutures, Bitfinex, Bitmart, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
MCOETH|7|49|Binance, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap
MCOBTC|6|36|Binance, Bittrex, Huobipro, Okex, Okexfutures, Okexswap
WTCBTC|6|36|Binance, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
WTCETH|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
LRCBTC|9|81|Binance, Bitfinex, Bittrex, Gateio, Okex, Okexfutures, Okexswap, Poloniex, Upbit
LRCETH|5|25|Binance, Gateio, Okex, Okexfutures, Okexswap
QTUMBTC|14|196|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
YOYOWBTC|4|16|Binance, Okex, Okexfutures, Okexswap
OMGBTC|15|225|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
OMGETH|10|100|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap
ZRXBTC|12|144|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ZRXETH|10|100|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
STRATBTC|4|16|Binance, Bittrex, Poloniex, Upbit
STRATETH|2|4|Binance, Bittrex
KNCBTC|9|81|Binance, Bitfinex, Coinbasepro, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
KNCETH|4|16|Binance, Gateio, Huobipro, Kucoin
FUNBTC|4|16|Binance, Okex, Okexfutures, Okexswap
FUNETH|3|9|Binance, Bitfinex, Gateio
NEOETH|7|49|Binance, Bitfinex, Bittrex, Kucoin, Okex, Okexfutures, Okexswap
IOTABTC|8|64|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap
IOTAETH|6|36|Binance, Bitfinex, Huobipro, Okex, Okexfutures, Okexswap
LINKBTC|11|121|Binance, Bittrex, Huobipro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
LINKETH|10|100|Binance, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Liquid, Okex, Okexfutures, Okexswap
XVGBTC|5|25|Binance, Bitfinex, Bittrex, Gateio, Huobipro
XVGETH|2|4|Binance, Huobipro
MTLBTC|4|16|Binance, Bittrex, Huobipro, Upbit
EOSBTC|14|196|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
SNTBTC|11|121|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ETCETH|9|81|Binance, Bittrex, Gateio, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
ETCBTC|14|196|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
ENGBTC|4|16|Binance, Bittrex, Huobipro, Upbit
ENGETH|2|4|Binance, Bittrex
DNTBTC|3|9|Binance, Bittrex, Upbit
ZECBTC|12|144|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
ZECETH|6|36|Binance, Bittrex, Okex, Okexfutures, Okexswap, Poloniex
BNTBTC|7|49|Binance, Bittrex, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ASTBTC|2|4|Binance, Huobipro
DASHBTC|15|225|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Zb
DASHETH|6|36|Binance, Bittrex, Kucoin, Okex, Okexfutures, Okexswap
OAXBTC|2|4|Binance, Gateio
BTGBTC|7|49|Binance, Bitfinex, Gateio, Huobipro, Okex, Okexfutures, Okexswap
EVXBTC|2|4|Binance, Huobipro
EVXETH|2|4|Binance, Huobipro
REQBTC|3|9|Binance, Huobipro, Kucoin
VIBBTC|6|36|Binance, Bittrex, Okex, Okexfutures, Okexswap, Upbit
VIBETH|2|4|Binance, Bittrex
TRXBTC|13|169|Binance, Bitfinex, Bittrex, Huobipro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
TRXETH|10|100|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap
POWRBTC|6|36|Binance, Bittrex, Gateio, Huobipro, Kucoin, Upbit
POWRETH|5|25|Binance, Bittrex, Gateio, Huobipro, Kucoin
ARKBTC|6|36|Binance, Bittrex, Okex, Okexfutures, Okexswap, Upbit
XRPBTC|17|289|Binance, Bitfinex, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
XRPETH|7|49|Binance, Bittrex, Kraken, Kucoin, Okex, Okexfutures, Okexswap
ENJBTC|4|16|Binance, Bittrex, Kucoin, Upbit
ENJETH|3|9|Binance, Bittrex, Kucoin
STORJBTC|6|36|Binance, Bittrex, Gateio, Huobipro, Poloniex, Upbit
STORJETH|5|25|Binance, Gateio, Okex, Okexfutures, Okexswap
BNBUSDT|6|36|Binance, Binancefutures, Ftx, Gateio, Kucoin, Poloniex
KMDBTC|5|25|Binance, Bittrex, Huobipro, Liquid, Upbit
KMDETH|2|4|Binance, Huobipro
RCNBTC|4|16|Binance, Bittrex, Huobipro, Upbit
NULSBTC|6|36|Binance, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
NULSETH|6|36|Binance, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
RDNBTC|2|4|Binance, Huobipro
XMRBTC|11|121|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
XMRETH|7|49|Binance, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
AMBBTC|2|4|Binance, Kucoin
BATBTC|11|121|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Okex, Okexfutures, Okexswap, Poloniex, Upbit
BATETH|8|64|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Poloniex
CDTETH|2|4|Binance, Gateio
GXSBTC|2|4|Binance, Gateio
NEOUSDT|11|121|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Zb
QSPBTC|2|4|Binance, Huobipro
QSPETH|2|4|Binance, Gateio
BTSBTC|8|64|Binance, Bittrex, Gateio, Huobipro, Indodax, Poloniex, Upbit, Zb
XZCBTC|3|9|Binance, Bittrex, Huobipro
XZCETH|2|4|Binance, Huobipro
LSKBTC|11|121|Binance, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
LSKETH|4|16|Binance, Huobipro, Kraken, Kucoin
TNTETH|2|4|Binance, Gateio
MANABTC|10|100|Binance, Bitfinex, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
MANAETH|8|64|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
BCDBTC|7|49|Binance, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
ADXBTC|4|16|Binance, Bittrex, Huobipro, Upbit
ADXETH|2|4|Binance, Bittrex
ADABTC|12|144|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Upbit, Zb
ADAETH|7|49|Binance, Bittrex, Huobipro, Kraken, Okex, Okexfutures, Okexswap
PPTBTC|2|4|Binance, Kucoin
CMTBTC|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
CMTETH|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
XLMBTC|16|256|Binance, Bitfinex, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
XLMETH|9|81|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
CNDBTC|2|4|Binance, Bittrex
LENDBTC|6|36|Binance, Huobipro, Okex, Okexfutures, Okexswap, Poloniex
LENDETH|6|36|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap
WABIBTC|2|4|Binance, Liquid
LTCETH|7|49|Binance, Bittrex, Kraken, Kucoin, Okex, Okexfutures, Okexswap
LTCUSDT|15|225|Binance, Binancefutures, Bitfinex, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
TNBBTC|3|9|Binance, Bitfinex, Huobipro
WAVESBTC|10|100|Binance, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Upbit
WAVESETH|7|49|Binance, Bittrex, Huobipro, Kraken, Okex, Okexfutures, Okexswap
GTOBTC|6|36|Binance, Bittrex, Okex, Okexfutures, Okexswap, Upbit
ICXBTC|7|49|Binance, Bittrex, Huobipro, Kraken, Okex, Okexfutures, Okexswap
ICXETH|4|16|Binance, Gateio, Huobipro, Kraken
OSTBTC|4|16|Binance, Bittrex, Huobipro, Upbit
OSTETH|2|4|Binance, Gateio
ELFBTC|8|64|Binance, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Upbit
ELFETH|7|49|Binance, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
AIONBTC|2|4|Binance, Kucoin
AIONETH|2|4|Binance, Kucoin
NEBLBTC|2|4|Binance, Kucoin
NAVBTC|2|4|Binance, Bittrex
APPCBTC|2|4|Binance, Huobipro
RLCBTC|4|16|Binance, Bitfinex, Bittrex, Upbit
RLCETH|2|4|Binance, Gateio
PIVXBTC|3|9|Binance, Bittrex, Kucoin
PIVXETH|2|4|Binance, Kucoin
IOSTBTC|8|64|Binance, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Upbit
IOSTETH|6|36|Binance, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
STEEMBTC|5|25|Binance, Bittrex, Huobipro, Poloniex, Upbit
STEEMETH|2|4|Binance, Huobipro
NANOBTC|8|64|Binance, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap
NANOETH|7|49|Binance, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap
VIABTC|2|4|Binance, Bittrex
BLZBTC|2|4|Binance, Huobipro
BLZETH|3|9|Binance, Gateio, Huobipro
AEBTC|3|9|Binance, Gateio, Huobipro
AEETH|3|9|Binance, Gateio, Huobipro
ZILBTC|8|64|Binance, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Upbit
ZILETH|7|49|Binance, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
ONTBTC|7|49|Binance, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
ONTETH|7|49|Binance, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
QTUMUSDT|9|81|Binance, Binancefutures, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex, Zb
XEMBTC|11|121|Binance, Bittrex, Gateio, Huobipro, Indodax, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
XEMETH|6|36|Binance, Bittrex, Gateio, Okex, Okexfutures, Okexswap
WANBTC|3|9|Binance, Huobipro, Kucoin
WANETH|3|9|Binance, Huobipro, Kucoin
WPRBTC|2|4|Binance, Huobipro
QLCBTC|2|4|Binance, Gateio
QLCETH|2|4|Binance, Gateio
SYSBTC|3|9|Binance, Bittrex, Upbit
GRSBTC|4|16|Binance, Bittrex, Huobipro, Upbit
ADAUSDT|12|144|Binance, Binancefutures, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Upbit, Zb
GNTBTC|9|81|Binance, Bitfinex, Bittrex, Huobipro, Okex, Okexfutures, Okexswap, Poloniex, Upbit
GNTETH|5|25|Binance, Bitfinex, Bittrex, Gateio, Huobipro
LOOMBTC|6|36|Binance, Bittrex, Huobipro, Kucoin, Poloniex, Upbit
LOOMETH|3|9|Binance, Huobipro, Kucoin
XRPUSDT|14|196|Binance, Binancefutures, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
REPBTC|6|36|Binance, Bitfinex, Coinbasepro, Kraken, Poloniex, Upbit
REPETH|3|9|Binance, Gateio, Kraken
BTCTUSD|2|4|Binance, Kucoin
ETHTUSD|2|4|Binance, Kucoin
ZENBTC|6|36|Binance, Bittrex, Huobipro, Okex, Okexfutures, Okexswap
ZENETH|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
EOSUSDT|12|144|Binance, Binancefutures, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Zb
CVCBTC|9|81|Binance, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
CVCETH|7|49|Binance, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap
THETABTC|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
THETAETH|3|9|Binance, Gateio, Huobipro
TUSDUSDT|9|81|Binance, Bitfinex, Bittrex, Gateio, Okex, Okexfutures, Okexswap, Upbit, Zb
IOTAUSDT|7|49|Binance, Binancefutures, Gateio, Huobipro, Okex, Okexfutures, Okexswap
XLMUSDT|11|121|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Zb
IOTXBTC|4|16|Binance, Bittrex, Kucoin, Upbit
IOTXETH|3|9|Binance, Gateio, Kucoin
QKCBTC|3|9|Binance, Gateio, Kucoin
QKCETH|3|9|Binance, Gateio, Kucoin
AGIBTC|2|4|Binance, Kucoin
NXSBTC|3|9|Binance, Bittrex, Upbit
DATABTC|2|4|Binance, Bitfinex
DATAETH|3|9|Binance, Bitfinex, Gateio
ONTUSDT|9|81|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
TRXUSDT|13|169|Binance, Binancefutures, Bittrex, Ftx, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
ETCUSDT|12|144|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
ICXUSDT|6|36|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap
SCBTC|9|81|Binance, Bittrex, Huobipro, Kraken, Okex, Okexfutures, Okexswap, Poloniex, Upbit
SCETH|7|49|Binance, Bittrex, Huobipro, Kraken, Okex, Okexfutures, Okexswap
NPXSETH|4|16|Binance, Bittrex, Huobipro, Kucoin
KEYETH|2|4|Binance, Kucoin
NASBTC|6|36|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap
NASETH|6|36|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap
DENTETH|2|4|Binance, Kucoin
ARDRBTC|8|64|Binance, Bittrex, Huobipro, Okex, Okexfutures, Okexswap, Poloniex, Upbit
NULSUSDT|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
VETBTC|6|36|Binance, Bitfinex, Bittrex, Huobipro, Kucoin, Upbit
VETETH|4|16|Binance, Gateio, Huobipro, Kucoin
VETUSDT|6|36|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Kucoin
DOCKBTC|3|9|Binance, Huobipro, Kucoin
POLYBTC|4|16|Binance, Huobipro, Poloniex, Upbit
HCBTC|8|64|Binance, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Zb
GOBTC|4|16|Binance, Bittrex, Kucoin, Upbit
PAXUSDT|8|64|Binance, Bitfinex, Gateio, Okex, Okexfutures, Okexswap, Poloniex, Zb
RVNBTC|7|49|Binance, Bittrex, Huobipro, Okex, Okexfutures, Okexswap, Upbit
DCRBTC|10|100|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
MITHBTC|4|16|Binance, Okex, Okexfutures, Okexswap
BCHBTC|16|256|Binance, Bitfinex, Bitflyer, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Upbit
BCHUSDT|15|225|Binance, Binancefutures, Bitfinex, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
BTCPAX|6|36|Binance, Bitmart, Bitstamp, Gateio, Kucoin, Poloniex
ETHPAX|4|16|Binance, Bitstamp, Kucoin, Poloniex
XRPPAX|3|9|Binance, Bitstamp, Kucoin
RENBTC|3|9|Binance, Huobipro, Poloniex
XRPTUSD|2|4|Binance, Kucoin
BTCUSDC|11|121|Binance, Bitmart, Coinbasepro, Gateio, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex
ETHUSDC|9|81|Binance, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex
XRPUSDC|5|25|Binance, Okex, Okexfutures, Okexswap, Poloniex
EOSUSDC|5|25|Binance, Okex, Okexfutures, Okexswap, Poloniex
USDCUSDT|9|81|Binance, Bitfinex, Bittrex, Gateio, Kraken, Okex, Okexfutures, Okexswap, Zb
LINKUSDT|14|196|Binance, Binancefutures, Bitfinex, Bittrex, Ftx, Gateio, Huobipro, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex, Zb
WAVESUSDT|8|64|Binance, Binancefutures, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
BCHUSDC|6|36|Binance, Liquid, Okex, Okexfutures, Okexswap, Poloniex
LTCUSDC|5|25|Binance, Okex, Okexfutures, Okexswap, Poloniex
TRXUSDC|5|25|Binance, Okex, Okexfutures, Okexswap, Poloniex
BTTUSDT|9|81|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
ONGBTC|2|4|Binance, Bittrex
ONGUSDT|2|4|Binance, Gateio
ZILUSDT|7|49|Binance, Binancefutures, Gateio, Huobipro, Okex, Okexfutures, Okexswap
ZRXUSDT|10|100|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex, Upbit
FETBTC|2|4|Binance, Kucoin
FETUSDT|2|4|Binance, Bitfinex
BATUSDT|10|100|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex, Upbit
XMRUSDT|10|100|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex, Zb
ZECUSDT|10|100|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
ZECUSDC|3|9|Binance, Coinbasepro, Poloniex
IOSTUSDT|6|36|Binance, Binancefutures, Huobipro, Okex, Okexfutures, Okexswap
CELRUSDT|2|4|Binance, Gateio
DASHUSDT|11|121|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Zb
NANOUSDT|7|49|Binance, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
OMGUSDT|10|100|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Upbit, Zb
THETAUSDT|7|49|Binance, Binancefutures, Gateio, Huobipro, Okex, Okexfutures, Okexswap
ENJUSDT|2|4|Binance, Bittrex
MITHUSDT|5|25|Binance, Gateio, Okex, Okexfutures, Okexswap
MATICBTC|2|4|Binance, Poloniex
MATICUSDT|2|4|Binance, Poloniex
ATOMBTC|13|169|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ATOMUSDT|10|100|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
ATOMUSDC|2|4|Binance, Poloniex
BATUSDC|2|4|Binance, Coinbasepro
TFUELUSDT|2|4|Binance, Gateio
ONEBTC|3|9|Binance, Huobipro, Kucoin
ONEUSDT|4|16|Binance, Gateio, Huobipro, Kucoin
FTMBTC|2|4|Binance, Kucoin
FTMUSDT|5|25|Binance, Gateio, Okex, Okexfutures, Okexswap
ALGOBTC|9|81|Binance, Bitfinex, Bittrex, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap
ALGOUSDT|10|100|Binance, Binancefutures, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
GTOUSDT|4|16|Binance, Okex, Okexfutures, Okexswap
DOGEBTC|9|81|Binance, Bittrex, Gateio, Huobipro, Indodax, Kraken, Poloniex, Upbit, Zb
DOGEUSDT|11|121|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex, Upbit, Zb
DUSKBTC|3|9|Binance, Bitfinex, Bittrex
ANKRBTC|4|16|Binance, Bittrex, Kucoin, Upbit
ANKRUSDT|2|4|Binance, Gateio
WINUSDT|4|16|Binance, Gateio, Kucoin, Poloniex
COSUSDT|2|4|Binance, Gateio
NPXSUSDT|2|4|Binance, Bittrex
COCOSUSDT|2|4|Binance, Gateio
MTLUSDT|2|4|Binance, Zb
TOMOBTC|2|4|Binance, Kucoin
TOMOUSDT|3|9|Binance, Gateio, Kucoin
DOCKUSDT|3|9|Binance, Gateio, Huobipro
FUNUSDT|2|4|Binance, Gateio
CVCUSDT|6|36|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap
BTTTRX|5|25|Binance, Gateio, Huobipro, Kucoin, Poloniex
WINTRX|3|9|Binance, Kucoin, Poloniex
CHZBTC|3|9|Binance, Kucoin, Upbit
CHZUSDT|2|4|Binance, Bitfinex
BANDBTC|3|9|Binance, Coinbasepro, Huobipro
BANDUSDT|5|25|Binance, Binancefutures, Gateio, Huobipro, Poloniex
BNBBUSD|2|4|Binance, Poloniex
BTCBUSD|2|4|Binance, Poloniex
BUSDUSDT|2|4|Binance, Poloniex
BEAMBTC|2|4|Binance, Gateio
BEAMUSDT|2|4|Binance, Gateio
XTZBTC|13|169|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
XTZUSDT|11|121|Binance, Binancefutures, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Zb
RENUSDT|4|16|Binance, Gateio, Huobipro, Poloniex
RVNUSDT|8|64|Binance, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Upbit
HCUSDT|7|49|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Zb
HBARBTC|6|36|Binance, Bittrex, Liquid, Okex, Okexfutures, Okexswap
HBARUSDT|6|36|Binance, Bittrex, Gateio, Okex, Okexfutures, Okexswap
NKNBTC|4|16|Binance, Bittrex, Huobipro, Upbit
NKNUSDT|3|9|Binance, Gateio, Huobipro
STXBTC|2|4|Binance, Kucoin
STXUSDT|3|9|Binance, Gateio, Kucoin
KAVABTC|2|4|Binance, Upbit
KAVAUSDT|3|9|Binance, Binancefutures, Gateio
BTCNGN|2|4|Binance, Coinbase
ARPABTC|2|4|Binance, Huobipro
ARPAUSDT|4|16|Binance, Gateio, Huobipro, Kucoin
IOTXUSDT|2|4|Binance, Gateio
RLCUSDT|3|9|Binance, Binancefutures, Gateio
MCOUSDT|6|36|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap
CTXCBTC|7|49|Binance, Bittrex, Huobipro, Okex, Okexfutures, Okexswap, Upbit
CTXCUSDT|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
BTCRUB|2|4|Binance, Coinbase
TROYUSDT|2|4|Binance, Gateio
VITEBTC|6|36|Binance, Bittrex, Okex, Okexfutures, Okexswap, Upbit
FTTBTC|3|9|Binance, Ftx, Huobipro
FTTUSDT|4|16|Binance, Bitfinex, Ftx, Huobipro
BTCTRY|2|4|Binance, Coinbase
BTCEUR|10|100|Binance, Bitfinex, Bitflyer, Bitstamp, Bittrex, Coinbase, Coinbasepro, Itbit, Kraken, Liquid
ETHEUR|8|64|Binance, Bitfinex, Bitstamp, Bittrex, Coinbasepro, Itbit, Kraken, Liquid
XRPEUR|5|25|Binance, Bitstamp, Coinbasepro, Kraken, Liquid
OGNBTC|4|16|Binance, Bittrex, Huobipro, Upbit
OGNUSDT|2|4|Binance, Huobipro
DREPUSDT|2|4|Binance, Gateio
TCTBTC|4|16|Binance, Okex, Okexfutures, Okexswap
TCTUSDT|5|25|Binance, Gateio, Okex, Okexfutures, Okexswap
WRXBTC|2|4|Binance, Poloniex
WRXUSDT|3|9|Binance, Ftx, Poloniex
BTSUSDT|4|16|Binance, Gateio, Huobipro, Zb
LSKUSDT|6|36|Binance, Gateio, Okex, Okexfutures, Okexswap, Poloniex
BNTUSDT|4|16|Binance, Okex, Okexfutures, Okexswap
MBLUSDT|2|4|Binance, Gateio
COTIBTC|2|4|Binance, Kucoin
COTIUSDT|3|9|Binance, Gateio, Kucoin
STPTBTC|4|16|Binance, Bittrex, Poloniex, Upbit
STPTUSDT|2|4|Binance, Poloniex
BTCZAR|2|4|Binance, Coinbase
WTCUSDT|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
DATAUSDT|2|4|Binance, Gateio
XZCUSDT|2|4|Binance, Huobipro
SOLBTC|2|4|Binance, Ftx
SOLUSDT|3|9|Binance, Ftx, Gateio
BTCIDRT|2|4|Binance, Liquid
CTSIBTC|2|4|Binance, Upbit
CTSIUSDT|2|4|Binance, Gateio
HIVEBTC|4|16|Binance, Bittrex, Huobipro, Upbit
HIVEUSDT|4|16|Binance, Bittrex, Gateio, Huobipro
CHRBTC|6|36|Binance, Bittrex, Huobipro, Kucoin, Poloniex, Upbit
CHRUSDT|4|16|Binance, Huobipro, Kucoin, Poloniex
GXSUSDT|2|4|Binance, Gateio
LENDUSDT|8|64|Binance, Binancefutures, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex
MDTBTC|7|49|Binance, Bittrex, Gateio, Okex, Okexfutures, Okexswap, Poloniex
MDTUSDT|7|49|Binance, Bittrex, Gateio, Okex, Okexfutures, Okexswap, Poloniex
STMXBTC|3|9|Binance, Bittrex, Upbit
STMXETH|2|4|Binance, Bittrex
KNCUSDT|8|64|Binance, Binancefutures, Ftx, Gateio, Huobipro, Okex, Okexfutures, Okexswap
REPUSDT|2|4|Binance, Poloniex
LRCUSDT|6|36|Binance, Gateio, Okex, Okexfutures, Okexswap, Poloniex
PNTBTC|2|4|Binance, Huobipro
BTCGBP|6|36|Binance, Bitfinex, Bitstamp, Coinbase, Coinbasepro, Kraken
ETHGBP|5|25|Binance, Bitfinex, Bitstamp, Coinbasepro, Kraken
XRPGBP|4|16|Binance, Bitstamp, Coinbasepro, Kraken
DGBBTC|9|81|Binance, Bitfinex, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Upbit
BTCUAH|2|4|Binance, Coinbase
COMPBTC|8|64|Binance, Bittrex, Coinbasepro, Huobipro, Okex, Okexfutures, Okexswap, Upbit
COMPUSDT|11|121|Binance, Binancefutures, Bittrex, Ftx, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
SCUSDT|7|49|Binance, Bittrex, Okex, Okexfutures, Okexswap, Poloniex, Upbit
ZENUSDT|4|16|Binance, Okex, Okexfutures, Okexswap
SXPBTC|5|25|Binance, Bittrex, Kucoin, Poloniex, Upbit
SNXBTC|4|16|Binance, Huobipro, Kucoin, Poloniex
SNXUSDT|9|81|Binance, Binancefutures, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
VTHOUSDT|2|4|Binance, Gateio
DGBUSDT|7|49|Binance, Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Upbit
SXPUSDT|6|36|Binance, Binancefutures, Ftx, Gateio, Kucoin, Poloniex
IRISBTC|3|9|Binance, Bittrex, Huobipro
MKRBTC|10|100|Binance, Bitfinex, Coinbasepro, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
MKRUSDT|10|100|Binance, Binancefutures, Ftx, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
DCRUSDT|8|64|Binance, Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Upbit
STORJUSDT|6|36|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap
BTCAUD|3|9|Binance, Coinbase, Liquid
ETHAUD|2|4|Binance, Liquid
AVABTC|3|9|Binance, Kucoin, Poloniex
MANAUSDT|7|49|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex
BALBTC|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
YFIBTC|2|4|Binance, Huobipro
YFIUSDT|5|25|Binance, Ftx, Gateio, Huobipro, Poloniex
BALUSDT|8|64|Binance, Ftx, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex
BLZUSDT|2|4|Binance, Gateio
IRISUSDT|4|16|Binance, Bittrex, Gateio, Huobipro
BTCDAI|8|64|Binance, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex
ETHDAI|9|81|Binance, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Okexfutures, Okexswap, Poloniex
USDTDAI|2|4|Binance, Kucoin
JSTBTC|3|9|Binance, Huobipro, Upbit
JSTUSDT|5|25|Binance, Gateio, Huobipro, Kucoin, Poloniex
SRMBTC|4|16|Binance, Okex, Okexfutures, Okexswap
SRMUSDT|6|36|Binance, Ftx, Gateio, Okex, Okexfutures, Okexswap
ANTBTC|8|64|Binance, Bitfinex, Bittrex, Huobipro, Okex, Okexfutures, Okexswap, Upbit
ANTUSDT|6|36|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap
CRVBTC|5|25|Binance, Huobipro, Okex, Okexfutures, Okexswap
CRVUSDT|7|49|Binance, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex
OCEANBTC|3|9|Binance, Bittrex, Kucoin
OCEANUSDT|4|16|Binance, Bittrex, Gateio, Poloniex
NMRBTC|5|25|Binance, Bittrex, Coinbasepro, Poloniex, Upbit
NMRUSDT|2|4|Binance, Bittrex
DOTBTC|8|64|Binance, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Upbit
DOTUSDT|12|144|Binance, Binancefutures, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Zb
LUNABTC|5|25|Binance, Bittrex, Huobipro, Kucoin, Upbit
LUNAUSDT|4|16|Binance, Bittrex, Huobipro, Kucoin
RSRBTC|3|9|Binance, Huobipro, Liquid
BTCUSD|12|144|Bitfinex, Bitflyer, Bitmex, Bitstamp, Bittrex, Bybit, Coinbase, Coinbasepro, Ftx, Itbit, Kraken, Liquid
LTCUSD|7|49|Bitfinex, Bitmex, Bitstamp, Bittrex, Coinbasepro, Ftx, Kraken
ETHUSD|10|100|Bitfinex, Bitmex, Bitstamp, Bittrex, Bybit, Coinbasepro, Ftx, Itbit, Kraken, Liquid
ETCUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
ZECUSD|3|9|Bitfinex, Bittrex, Kraken
XMRUSD|2|4|Bitfinex, Kraken
DASHUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
BTCJPY|6|36|Bitfinex, Bitflyer, Coinbase, Coincheck, Kraken, Liquid
XRPUSD|9|81|Bitfinex, Bitmex, Bitstamp, Bittrex, Bybit, Coinbasepro, Ftx, Kraken, Liquid
EOSUSD|5|25|Bitfinex, Bittrex, Bybit, Coinbasepro, Kraken
OMGUSD|3|9|Bitfinex, Coinbasepro, Kraken
QTUMUSD|2|4|Bitfinex, Kraken
QASHUSD|2|4|Bitfinex, Liquid
BATUSD|3|9|Bitfinex, Bittrex, Kraken
ZRXUSD|3|9|Bitfinex, Bittrex, Coinbasepro
TRXUSD|4|16|Bitfinex, Bittrex, Ftx, Kraken
REPUSD|3|9|Bitfinex, Coinbasepro, Kraken
ETHJPY|4|16|Bitfinex, Bitflyer, Kraken, Liquid
EOSEUR|3|9|Bitfinex, Coinbasepro, Kraken
WAXPUSD|2|4|Bitfinex, Bittrex
WAXPBTC|5|25|Bitfinex, Bittrex, Huobipro, Kucoin, Upbit
DAIUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
DAIBTC|3|9|Bitfinex, Bittrex, Upbit
DAIETH|2|4|Bitfinex, Bittrex
ANTETH|3|9|Bitfinex, Bittrex, Huobipro
XLMUSD|5|25|Bitfinex, Bitstamp, Bittrex, Coinbasepro, Kraken
XLMEUR|4|16|Bitfinex, Bitstamp, Coinbasepro, Kraken
XLMGBP|2|4|Bitfinex, Bitstamp
MKRUSD|3|9|Bitfinex, Coinbasepro, Ftx
MKRETH|7|49|Bitfinex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
KNCUSD|3|9|Bitfinex, Coinbasepro, Ftx
XTZUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
TRXEUR|3|9|Bitfinex, Bittrex, Kraken
MLNUSD|2|4|Bitfinex, Kraken
PNKETH|4|16|Bitfinex, Okex, Okexfutures, Okexswap
DGBUSD|2|4|Bitfinex, Bittrex
BSVUSD|2|4|Bitfinex, Bittrex
BSVBTC|10|100|Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Upbit
BCHUSD|8|64|Bitfinex, Bitmex, Bitstamp, Bittrex, Coinbasepro, Ftx, Kraken, Liquid
ENJUSD|2|4|Bitfinex, Bittrex
USDTUSD|4|16|Bitfinex, Bittrex, Ftx, Kraken
USDCUSD|3|9|Bitfinex, Bittrex, Kraken
TUSDUSD|2|4|Bitfinex, Bittrex
PAXUSD|3|9|Bitfinex, Bitstamp, Bittrex
RIFUSD|2|4|Bitfinex, Liquid
RIFBTC|3|9|Bitfinex, Kucoin, Liquid
VSYSBTC|7|49|Bitfinex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Zb
BTTBTC|8|64|Bitfinex, Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Upbit
GNOUSD|2|4|Bitfinex, Kraken
ATOMUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
ATOMETH|8|64|Bitfinex, Bittrex, Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap
LEOBTC|5|25|Bitfinex, Gateio, Okex, Okexfutures, Okexswap
LEOUSDT|6|36|Bitfinex, Gateio, Okex, Okexfutures, Okexswap, Zb
LEOETH|4|16|Bitfinex, Okex, Okexfutures, Okexswap
OKBUSDT|5|25|Bitfinex, Gateio, Okex, Okexfutures, Okexswap
KANUSDT|5|25|Bitfinex, Huobipro, Okex, Okexfutures, Okexswap
AMPLUSD|2|4|Bitfinex, Ftx
ALGOUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
AMPLUSDT|4|16|Bitfinex, Ftx, Gateio, Kucoin
AMPLBTC|2|4|Bitfinex, Kucoin
FTTUSD|2|4|Bitfinex, Ftx
XAUTUSD|2|4|Bitfinex, Ftx
XAUTUSDT|2|4|Bitfinex, Ftx
DOTUSD|2|4|Bitfinex, Bittrex
ADAUSD|3|9|Bitfinex, Bittrex, Kraken
LINKUSD|5|25|Bitfinex, Bittrex, Coinbasepro, Ftx, Kraken
BTCKRW|3|9|Bithumb, Coinbase, Upbit
ETHKRW|2|4|Bithumb, Upbit
LTCKRW|2|4|Bithumb, Upbit
ETCKRW|2|4|Bithumb, Upbit
XRPKRW|2|4|Bithumb, Upbit
BCHKRW|2|4|Bithumb, Upbit
QTUMKRW|2|4|Bithumb, Upbit
BTGKRW|2|4|Bithumb, Upbit
EOSKRW|2|4|Bithumb, Upbit
ICXKRW|2|4|Bithumb, Upbit
TRXKRW|2|4|Bithumb, Upbit
ELFKRW|2|4|Bithumb, Upbit
OMGKRW|2|4|Bithumb, Upbit
KNCKRW|2|4|Bithumb, Upbit
GNTKRW|2|4|Bithumb, Upbit
ZILKRW|2|4|Bithumb, Upbit
WAXPKRW|2|4|Bithumb, Upbit
POWRKRW|2|4|Bithumb, Upbit
STEEMKRW|2|4|Bithumb, Upbit
STRATKRW|2|4|Bithumb, Upbit
ZRXKRW|2|4|Bithumb, Upbit
REPKRW|2|4|Bithumb, Upbit
XEMKRW|2|4|Bithumb, Upbit
SNTKRW|2|4|Bithumb, Upbit
ADAKRW|2|4|Bithumb, Upbit
BATKRW|2|4|Bithumb, Upbit
THETAKRW|2|4|Bithumb, Upbit
LOOMKRW|2|4|Bithumb, Upbit
WAVESKRW|2|4|Bithumb, Upbit
LINKKRW|2|4|Bithumb, Upbit
ENJKRW|2|4|Bithumb, Upbit
VETKRW|2|4|Bithumb, Upbit
MTLKRW|2|4|Bithumb, Upbit
IOSTKRW|2|4|Bithumb, Upbit
QKCKRW|2|4|Bithumb, Upbit
NPXSKRW|2|4|Bithumb, Upbit
BSVKRW|2|4|Bithumb, Upbit
ORBSKRW|2|4|Bithumb, Upbit
ANKRKRW|2|4|Bithumb, Upbit
CROKRW|2|4|Bithumb, Upbit
MBLKRW|2|4|Bithumb, Upbit
HIVEKRW|2|4|Bithumb, Upbit
BORAKRW|2|4|Bithumb, Upbit
XLMKRW|2|4|Bithumb, Upbit
BTTKRW|2|4|Bithumb, Upbit
XTZKRW|2|4|Bithumb, Upbit
GBPUSD|2|4|Bitstamp, Kraken
EURUSD|2|4|Bitstamp, Kraken
LTCEUR|3|9|Bitstamp, Coinbasepro, Kraken
LTCGBP|3|9|Bitstamp, Coinbasepro, Kraken
BCHEUR|4|16|Bitstamp, Bittrex, Coinbasepro, Kraken
BCHGBP|3|9|Bitstamp, Coinbasepro, Kraken
AKROBTC|3|9|Bittrex, Huobipro, Kucoin
APIXBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
APMBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
APMUSDT|4|16|Bittrex, Okex, Okexfutures, Okexswap
BCHETH|3|9|Bittrex, Kraken, Kucoin
BFTBTC|3|9|Bittrex, Huobipro, Upbit
BLKBTC|2|4|Bittrex, Upbit
BORABTC|2|4|Bittrex, Upbit
BSVETH|2|4|Bittrex, Kucoin
BSVUSDT|9|81|Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Poloniex, Zb
BTMBTC|8|64|Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Upbit
BTUBTC|2|4|Bittrex, Upbit
BURSTBTC|2|4|Bittrex, Upbit
CELOBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
CELOUSDT|4|16|Bittrex, Okex, Okexfutures, Okexswap
CKBBTC|3|9|Bittrex, Gateio, Huobipro
CKBUSDT|3|9|Bittrex, Gateio, Huobipro
CMCTBTC|2|4|Bittrex, Upbit
COMPETH|3|9|Bittrex, Huobipro, Poloniex
COMPUSD|3|9|Bittrex, Coinbasepro, Ftx
CPCBTC|2|4|Bittrex, Kucoin
CROBTC|8|64|Bittrex, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Upbit, Zb
CROUSDT|8|64|Bittrex, Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap, Zb
CRWBTC|2|4|Bittrex, Upbit
CTCBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
CVTBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
DAIUSDT|8|64|Bittrex, Gateio, Huobipro, Kraken, Okex, Okexfutures, Okexswap, Poloniex
DENTBTC|3|9|Bittrex, Kucoin, Upbit
DEPUSDT|4|16|Bittrex, Okex, Okexfutures, Okexswap
DGBETH|3|9|Bittrex, Huobipro, Kucoin
DMTBTC|2|4|Bittrex, Upbit
DNABTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
DNAUSDT|5|25|Bittrex, Okex, Okexfutures, Okexswap, Zb
DOGEETH|2|4|Bittrex, Huobipro
DOGEUSD|2|4|Bittrex, Kraken
DOTETH|4|16|Bittrex, Okex, Okexfutures, Okexswap
DRGNBTC|2|4|Bittrex, Kucoin
DTABTC|3|9|Bittrex, Huobipro, Upbit
EDRBTC|2|4|Bittrex, Upbit
EMC2BTC|2|4|Bittrex, Upbit
EXPBTC|2|4|Bittrex, Upbit
FCTBTC|2|4|Bittrex, Liquid
FORBTC|2|4|Bittrex, Huobipro
FSNBTC|3|9|Bittrex, Huobipro, Upbit
FXBTC|3|9|Bittrex, Kucoin, Upbit
FXCBTC|2|4|Bittrex, Poloniex
FXETH|2|4|Bittrex, Kucoin
GBYTEBTC|2|4|Bittrex, Upbit
GNOBTC|2|4|Bittrex, Kraken
GNOETH|2|4|Bittrex, Kraken
GRINBTC|3|9|Bittrex, Gateio, Kucoin
GRINUSDT|4|16|Bittrex, Gateio, Kucoin, Poloniex
GXCBTC|2|4|Bittrex, Huobipro
GXCUSDT|2|4|Bittrex, Huobipro
HBARETH|2|4|Bittrex, Liquid
HBARUSD|2|4|Bittrex, Liquid
HBDBTC|2|4|Bittrex, Upbit
HDAOUSDT|4|16|Bittrex, Okex, Okexfutures, Okexswap
HNSBTC|2|4|Bittrex, Gateio
HNSUSDT|3|9|Bittrex, Gateio, Zb
HYCBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
IGNISBTC|2|4|Bittrex, Upbit
JNTBTC|3|9|Bittrex, Gateio, Upbit
KSMBTC|3|9|Bittrex, Huobipro, Kucoin
KSMUSDT|4|16|Bittrex, Gateio, Huobipro, Kucoin
LAMBBTC|3|9|Bittrex, Huobipro, Upbit
LBABTC|6|36|Bittrex, Huobipro, Okex, Okexfutures, Okexswap, Upbit
LBCBTC|2|4|Bittrex, Upbit
MEDBTC|2|4|Bittrex, Upbit
METABTC|3|9|Bittrex, Kucoin, Upbit
METETH|2|4|Bittrex, Gateio
MFTBTC|2|4|Bittrex, Upbit
MOCBTC|2|4|Bittrex, Upbit
MOFBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
MOFUSDT|4|16|Bittrex, Okex, Okexfutures, Okexswap
NPXSBTC|4|16|Bittrex, Huobipro, Kucoin, Upbit
NXTBTC|4|16|Bittrex, Indodax, Poloniex, Upbit
ORBSBTC|2|4|Bittrex, Upbit
OXTBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
OXTUSDT|4|16|Bittrex, Okex, Okexfutures, Okexswap
PAXBTC|5|25|Bittrex, Okex, Okexfutures, Okexswap, Upbit
PAYBTC|7|49|Bittrex, Gateio, Huobipro, Okex, Okexfutures, Okexswap, Upbit
PAYETH|3|9|Bittrex, Gateio, Huobipro
PIBTC|2|4|Bittrex, Upbit
PMABTC|5|25|Bittrex, Okex, Okexfutures, Okexswap, Upbit
PXLBTC|2|4|Bittrex, Upbit
QNTBTC|2|4|Bittrex, Upbit
QRLBTC|2|4|Bittrex, Upbit
RADSBTC|2|4|Bittrex, Upbit
RDDBTC|2|4|Bittrex, Upbit
RFRBTC|2|4|Bittrex, Upbit
SBDBTC|2|4|Bittrex, Upbit
SCUSD|2|4|Bittrex, Kraken
SENSOBTC|2|4|Bittrex, Kucoin
SIXBTC|2|4|Bittrex, Liquid
SKMBTC|2|4|Bittrex, Huobipro
SKMUSDT|3|9|Bittrex, Gateio, Huobipro
SOLVEBTC|3|9|Bittrex, Kucoin, Upbit
SPCBTC|2|4|Bittrex, Upbit
SPNDBTC|6|36|Bittrex, Kucoin, Okex, Okexfutures, Okexswap, Upbit
SRNBTC|3|9|Bittrex, Huobipro, Upbit
SRNETH|2|4|Bittrex, Huobipro
SUKUBTC|2|4|Bittrex, Kucoin
SUKUUSDT|2|4|Bittrex, Kucoin
SUTERBTC|2|4|Bittrex, Kucoin
SUTERUSDT|3|9|Bittrex, Gateio, Kucoin
TNCBTC|2|4|Bittrex, Gateio
TRACBTC|2|4|Bittrex, Kucoin
TRACETH|2|4|Bittrex, Kucoin
TSHPBTC|2|4|Bittrex, Upbit
TTCBTC|2|4|Bittrex, Upbit
TUSDBTC|5|25|Bittrex, Okex, Okexfutures, Okexswap, Upbit
UBTBTC|2|4|Bittrex, Liquid
UPPBTC|2|4|Bittrex, Upbit
USDCBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
USDTEUR|2|4|Bittrex, Kraken
UTKBTC|3|9|Bittrex, Huobipro, Kucoin
VDXBTC|2|4|Bittrex, Upbit
VEEBTC|2|4|Bittrex, Upbit
VIDBTC|2|4|Bittrex, Kucoin
VRABTC|2|4|Bittrex, Kucoin
VTCBTC|2|4|Bittrex, Upbit
WAXPETH|3|9|Bittrex, Huobipro, Kucoin
WAXPUSDT|2|4|Bittrex, Huobipro
WICCBTC|2|4|Bittrex, Huobipro
WICCUSDT|3|9|Bittrex, Gateio, Huobipro
XDNBTC|2|4|Bittrex, Upbit
XSRBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
XTZETH|4|16|Bittrex, Gateio, Huobipro, Kraken
XUCUSDT|4|16|Bittrex, Okex, Okexfutures, Okexswap
XVGUSDT|2|4|Bittrex, Gateio
YOUBTC|4|16|Bittrex, Okex, Okexfutures, Okexswap
BTCBRL|2|4|Coinbase, Ftx
BTCCAD|2|4|Coinbase, Kraken
BTCCHF|2|4|Coinbase, Kraken
BTCHKD|2|4|Coinbase, Liquid
BTCIDR|2|4|Coinbase, Indodax
BTCSGD|3|9|Coinbase, Itbit, Liquid
LINKEUR|2|4|Coinbasepro, Kraken
ETCEUR|2|4|Coinbasepro, Kraken
ALGOEUR|2|4|Coinbasepro, Kraken
OMGEUR|2|4|Coinbasepro, Kraken
XTZEUR|2|4|Coinbasepro, Kraken
CUSDTUSDT|2|4|Ftx, Poloniex
DMGUSDT|6|36|Ftx, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
MTAUSDT|3|9|Ftx, Gateio, Poloniex
PAXGUSD|2|4|Ftx, Kraken
BCHBEARUSDT|2|4|Ftx, Poloniex
BCHBULLUSDT|2|4|Ftx, Poloniex
BEARUSDT|3|9|Ftx, Gateio, Poloniex
BSVBEARUSDT|2|4|Ftx, Poloniex
BSVBULLUSDT|2|4|Ftx, Poloniex
BULLUSDT|3|9|Ftx, Gateio, Poloniex
BVOLUSDT|2|4|Ftx, Poloniex
EOSBEARUSDT|3|9|Ftx, Gateio, Poloniex
EOSBULLUSDT|3|9|Ftx, Gateio, Poloniex
ETHBEARUSDT|3|9|Ftx, Gateio, Poloniex
ETHBULLUSDT|3|9|Ftx, Gateio, Poloniex
IBVOLUSDT|2|4|Ftx, Poloniex
LINKBEARUSDT|2|4|Ftx, Poloniex
LINKBULLUSDT|2|4|Ftx, Poloniex
XRPBEARUSDT|3|9|Ftx, Gateio, Poloniex
XRPBULLUSDT|3|9|Ftx, Gateio, Poloniex
BTMUSDT|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
SNTUSDT|6|36|Gateio, Huobipro, Okex, Okexfutures, Okexswap, Zb
PAYUSDT|4|16|Gateio, Okex, Okexfutures, Okexswap
PSTUSDT|4|16|Gateio, Okex, Okexfutures, Okexswap
BTGUSDT|4|16|Gateio, Okex, Okexfutures, Okexswap
AEUSDT|2|4|Gateio, Huobipro
REQETH|3|9|Gateio, Huobipro, Kucoin
MDAUSDT|4|16|Gateio, Okex, Okexfutures, Okexswap
GNTUSDT|7|49|Gateio, Huobipro, Okex, Okexfutures, Okexswap, Poloniex, Zb
ABTUSDT|4|16|Gateio, Okex, Okexfutures, Okexswap
ABTETH|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
OCNUSDT|2|4|Gateio, Huobipro
OCNETH|2|4|Gateio, Huobipro
OCNBTC|2|4|Gateio, Huobipro
COFIETH|2|4|Gateio, Kucoin
RUFFUSDT|2|4|Gateio, Huobipro
RUFFETH|2|4|Gateio, Huobipro
RUFFBTC|2|4|Gateio, Huobipro
SMTUSDT|2|4|Gateio, Huobipro
SMTETH|2|4|Gateio, Huobipro
MDTETH|4|16|Gateio, Okex, Okexfutures, Okexswap
ELFUSDT|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
DRGNETH|2|4|Gateio, Kucoin
GTCETH|2|4|Gateio, Huobipro
GTCBTC|2|4|Gateio, Huobipro
DBCBTC|3|9|Gateio, Huobipro, Kucoin
DBCETH|3|9|Gateio, Huobipro, Kucoin
BIFIBTC|2|4|Gateio, Huobipro
MDSETH|2|4|Gateio, Huobipro
MDSUSDT|2|4|Gateio, Huobipro
DGDETH|2|4|Gateio, Huobipro
QASHETH|3|9|Gateio, Huobipro, Liquid
QASHBTC|3|9|Gateio, Huobipro, Liquid
BCDUSDT|4|16|Gateio, Okex, Okexfutures, Okexswap
SBTCBTC|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
BCXBTC|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
GNXETH|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
GASUSDT|4|16|Gateio, Okex, Okexfutures, Okexswap
NASUSDT|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
BTMETH|6|36|Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
GTBTC|2|4|Gateio, Huobipro
GTUSDT|2|4|Gateio, Huobipro
RSRUSDT|3|9|Gateio, Huobipro, Liquid
KAIUSDT|2|4|Gateio, Kucoin
WNXMUSDT|2|4|Gateio, Huobipro
SWAPUSDT|2|4|Gateio, Poloniex
ASTUSDT|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
OMUSDT|5|25|Gateio, Okex, Okexfutures, Okexswap, Poloniex
AKROUSDT|3|9|Gateio, Huobipro, Kucoin
FORUSDT|2|4|Gateio, Huobipro
DIAUSDT|6|36|Gateio, Kucoin, Okex, Okexfutures, Okexswap, Poloniex
TRBUSDT|3|9|Gateio, Huobipro, Poloniex
DOSUSDT|2|4|Gateio, Poloniex
XEMUSDT|6|36|Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
BUETH|2|4|Gateio, Kucoin
BUBTC|2|4|Gateio, Kucoin
BTC3LUSDT|3|9|Gateio, Huobipro, Liquid
BTC3SUSDT|3|9|Gateio, Huobipro, Liquid
ETH3LUSDT|2|4|Gateio, Liquid
ETH3SUSDT|2|4|Gateio, Liquid
BCNUSDT|2|4|Gateio, Poloniex
STEEMUSDT|3|9|Gateio, Huobipro, Poloniex
ATPUSDT|2|4|Gateio, Huobipro
KLAYUSDT|2|4|Gateio, Liquid
GRINETH|2|4|Gateio, Kucoin
BTTETH|6|36|Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
CSETH|2|4|Gateio, Kucoin
MANETH|3|9|Gateio, Huobipro, Kucoin
LYMETH|3|9|Gateio, Huobipro, Kucoin
LYMBTC|3|9|Gateio, Huobipro, Kucoin
LYMUSDT|2|4|Gateio, Kucoin
BFTETH|2|4|Gateio, Huobipro
TOMOETH|2|4|Gateio, Kucoin
SOULETH|2|4|Gateio, Kucoin
DOCKETH|3|9|Gateio, Huobipro, Kucoin
HITUSDT|2|4|Gateio, Huobipro
HITETH|2|4|Gateio, Huobipro
DXETH|2|4|Gateio, Kucoin
CNNSUSDT|2|4|Gateio, Huobipro
LAMBUSDT|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
LAMBETH|2|4|Gateio, Huobipro
WICCETH|2|4|Gateio, Huobipro
VIDYUSDT|2|4|Gateio, Huobipro
FTMETH|2|4|Gateio, Kucoin
MTVUSDT|2|4|Gateio, Kucoin
HCETH|6|36|Gateio, Huobipro, Kucoin, Okex, Okexfutures, Okexswap
FTIETH|2|4|Gateio, Huobipro
LBAUSDT|5|25|Gateio, Huobipro, Okex, Okexfutures, Okexswap
LBAETH|2|4|Gateio, Huobipro
OPENETH|2|4|Gateio, Kucoin
MITHETH|4|16|Gateio, Okex, Okexfutures, Okexswap
HTUSDT|2|4|Gateio, Huobipro
MXCBTC|2|4|Gateio, Huobipro
SNCBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
QUNBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
LETBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
KANBTC|5|25|Huobipro, Okex, Okexfutures, Okexswap, Zb
ABTBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
SWFTCBTC|5|25|Huobipro, Okex, Okexfutures, Okexswap, Poloniex
WXTBTC|5|25|Huobipro, Kucoin, Okex, Okexfutures, Okexswap
KCASHETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
TOPCETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
TRIOETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
MANBTC|2|4|Huobipro, Kucoin
LETUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
AACETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
DATXETH|2|4|Huobipro, Kucoin
SNXETH|5|25|Huobipro, Kucoin, Okex, Okexfutures, Okexswap
AACUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
KCASHUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
GASETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
ETNETH|3|9|Huobipro, Kucoin, Liquid
WXTUSDT|5|25|Huobipro, Kucoin, Okex, Okexfutures, Okexswap
ELABTC|2|4|Huobipro, Kucoin
SWFTCETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
CTXCETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
ITCUSDT|5|25|Huobipro, Kucoin, Okex, Okexfutures, Okexswap
FAIRETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
AACBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
YEEUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
ACTUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
TRIOBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
ACTBTC|5|25|Huobipro, Kucoin, Okex, Okexfutures, Okexswap
CRVETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
EMUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
KANETH|4|16|Huobipro, Okex, Okexfutures, Okexswap
EGTUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
EGTBTC|5|25|Huobipro, Kucoin, Okex, Okexfutures, Okexswap
ALGOETH|6|36|Huobipro, Kraken, Kucoin, Okex, Okexfutures, Okexswap
DCRETH|2|4|Huobipro, Kucoin
ITCBTC|5|25|Huobipro, Kucoin, Okex, Okexfutures, Okexswap
CHATBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
ETNBTC|3|9|Huobipro, Kucoin, Liquid
ITCETH|2|4|Huobipro, Kucoin
MTNBTC|2|4|Huobipro, Kucoin
SOCBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
CMTUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
UTKETH|2|4|Huobipro, Kucoin
ELAETH|2|4|Huobipro, Kucoin
NCASHBTC|2|4|Huobipro, Upbit
FSNUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
BALETH|2|4|Huobipro, Poloniex
KCASHBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
ACTETH|2|4|Huobipro, Kucoin
GNXBTC|4|16|Huobipro, Okex, Okexfutures, Okexswap
DATXBTC|2|4|Huobipro, Kucoin
SOCUSDT|4|16|Huobipro, Okex, Okexfutures, Okexswap
VSYSUSDT|5|25|Huobipro, Kucoin, Okex, Okexfutures, Okexswap
ETHSGD|2|4|Itbit, Liquid
XRPJPY|2|4|Kraken, Liquid
EGTETH|4|16|Kucoin, Okex, Okexfutures, Okexswap
CRPTETH|2|4|Kucoin, Liquid
MTCBTC|2|4|Kucoin, Liquid
CRPTBTC|2|4|Kucoin, Liquid
USDTUSDC|2|4|Kucoin, Poloniex
AVAUSDT|2|4|Kucoin, Poloniex
BLOCUSDT|4|16|Kucoin, Okex, Okexfutures, Okexswap
ROOBEEBTC|2|4|Kucoin, Liquid
ROADUSDT|4|16|Kucoin, Okex, Okexfutures, Okexswap
WOMUSDT|2|4|Kucoin, Liquid
XSRUSDT|4|16|Kucoin, Okex, Okexfutures, Okexswap
EWTBTC|2|4|Kucoin, Liquid
PLTUSDT|2|4|Kucoin, Poloniex
MLKBTC|2|4|Kucoin, Upbit
AERGOBTC|5|25|Kucoin, Okex, Okexfutures, Okexswap, Upbit
PCIBTC|2|4|Liquid, Upbit
GOM2BTC|2|4|Liquid, Upbit
XPOUSDT|3|9|Okex, Okexfutures, Okexswap
ROADUSDK|3|9|Okex, Okexfutures, Okexswap
HDAOUSDK|3|9|Okex, Okexfutures, Okexswap
DIAETH|3|9|Okex, Okexfutures, Okexswap
PNKUSDT|3|9|Okex, Okexfutures, Okexswap
OMETH|3|9|Okex, Okexfutures, Okexswap
XPRBTC|3|9|Okex, Okexfutures, Okexswap
AETBTC|3|9|Okex, Okexfutures, Okexswap
BHPBTC|3|9|Okex, Okexfutures, Okexswap
GUSDBTC|3|9|Okex, Okexfutures, Okexswap
IQBTC|3|9|Okex, Okexfutures, Okexswap
ORSBTC|3|9|Okex, Okexfutures, Okexswap
TMTGBTC|3|9|Okex, Okexfutures, Okexswap
INTBTC|3|9|Okex, Okexfutures, Okexswap
PSTBTC|3|9|Okex, Okexfutures, Okexswap
TRUEBTC|4|16|Okex, Okexfutures, Okexswap, Zb
OKBBTC|3|9|Okex, Okexfutures, Okexswap
AETETH|3|9|Okex, Okexfutures, Okexswap
HYCETH|3|9|Okex, Okexfutures, Okexswap
ORSETH|3|9|Okex, Okexfutures, Okexswap
YOUETH|3|9|Okex, Okexfutures, Okexswap
INTETH|3|9|Okex, Okexfutures, Okexswap
MOFETH|3|9|Okex, Okexfutures, Okexswap
TRUEETH|3|9|Okex, Okexfutures, Okexswap
GTOETH|3|9|Okex, Okexfutures, Okexswap
OKBETH|3|9|Okex, Okexfutures, Okexswap
BTCUSDK|3|9|Okex, Okexfutures, Okexswap
LTCUSDK|3|9|Okex, Okexfutures, Okexswap
ETHUSDK|3|9|Okex, Okexfutures, Okexswap
OKBUSDK|3|9|Okex, Okexfutures, Okexswap
ETCUSDK|3|9|Okex, Okexfutures, Okexswap
BCHUSDK|3|9|Okex, Okexfutures, Okexswap
EOSUSDK|3|9|Okex, Okexfutures, Okexswap
XRPUSDK|3|9|Okex, Okexfutures, Okexswap
TRXUSDK|3|9|Okex, Okexfutures, Okexswap
BSVUSDK|3|9|Okex, Okexfutures, Okexswap
USDTUSDK|3|9|Okex, Okexfutures, Okexswap
ALGOUSDK|3|9|Okex, Okexfutures, Okexswap
CROUSDK|3|9|Okex, Okexfutures, Okexswap
DEPUSDK|3|9|Okex, Okexfutures, Okexswap
DOGEUSDK|3|9|Okex, Okexfutures, Okexswap
ECUSDK|3|9|Okex, Okexfutures, Okexswap
EMUSDK|3|9|Okex, Okexfutures, Okexswap
FSNUSDK|3|9|Okex, Okexfutures, Okexswap
FTMUSDK|3|9|Okex, Okexfutures, Okexswap
HBARUSDK|3|9|Okex, Okexfutures, Okexswap
LAMBUSDK|3|9|Okex, Okexfutures, Okexswap
LEOUSDK|3|9|Okex, Okexfutures, Okexswap
NDNUSDK|3|9|Okex, Okexfutures, Okexswap
ORBSUSDK|3|9|Okex, Okexfutures, Okexswap
PLGUSDK|3|9|Okex, Okexfutures, Okexswap
PMAUSDK|3|9|Okex, Okexfutures, Okexswap
VSYSUSDK|3|9|Okex, Okexfutures, Okexswap
WGRTUSDK|3|9|Okex, Okexfutures, Okexswap
WXTUSDK|3|9|Okex, Okexfutures, Okexswap
TRXOKB|3|9|Okex, Okexfutures, Okexswap
XPRUSDT|3|9|Okex, Okexfutures, Okexswap
AETUSDT|3|9|Okex, Okexfutures, Okexswap
AERGOUSDT|3|9|Okex, Okexfutures, Okexswap
ALVUSDT|3|9|Okex, Okexfutures, Okexswap
APIXUSDT|3|9|Okex, Okexfutures, Okexswap
BHPUSDT|3|9|Okex, Okexfutures, Okexswap
CTCUSDT|3|9|Okex, Okexfutures, Okexswap
CVTUSDT|3|9|Okex, Okexfutures, Okexswap
ECUSDT|3|9|Okex, Okexfutures, Okexswap
ETMUSDT|3|9|Okex, Okexfutures, Okexswap
GUSDUSDT|4|16|Okex, Okexfutures, Okexswap, Zb
HYCUSDT|3|9|Okex, Okexfutures, Okexswap
IQUSDT|3|9|Okex, Okexfutures, Okexswap
NDNUSDT|3|9|Okex, Okexfutures, Okexswap
ORBSUSDT|3|9|Okex, Okexfutures, Okexswap
ORSUSDT|3|9|Okex, Okexfutures, Okexswap
PLGUSDT|3|9|Okex, Okexfutures, Okexswap
TMTGUSDT|3|9|Okex, Okexfutures, Okexswap
WGRTUSDT|3|9|Okex, Okexfutures, Okexswap
YOUUSDT|3|9|Okex, Okexfutures, Okexswap
EGTOKB|3|9|Okex, Okexfutures, Okexswap
SCOKB|3|9|Okex, Okexfutures, Okexswap
WXTOKB|3|9|Okex, Okexfutures, Okexswap
DASHOKB|3|9|Okex, Okexfutures, Okexswap
ARKUSDT|3|9|Okex, Okexfutures, Okexswap
YOYOWUSDT|3|9|Okex, Okexfutures, Okexswap
PPTUSDT|3|9|Okex, Okexfutures, Okexswap
SWFTCUSDT|5|25|Okex, Okexfutures, Okexswap, Poloniex, Zb
RNTUSDT|3|9|Okex, Okexfutures, Okexswap
FAIRUSDT|3|9|Okex, Okexfutures, Okexswap
UBTCUSDT|3|9|Okex, Okexfutures, Okexswap
VIBUSDT|3|9|Okex, Okexfutures, Okexswap
UTKUSDT|3|9|Okex, Okexfutures, Okexswap
TOPCUSDT|4|16|Okex, Okexfutures, Okexswap, Zb
QUNUSDT|3|9|Okex, Okexfutures, Okexswap
INTUSDT|3|9|Okex, Okexfutures, Okexswap
TRUEUSDT|4|16|Okex, Okexfutures, Okexswap, Zb
ZIPUSDT|3|9|Okex, Okexfutures, Okexswap
CHATUSDT|4|16|Okex, Okexfutures, Okexswap, Zb
BECUSDT|3|9|Okex, Okexfutures, Okexswap
TRIOUSDT|3|9|Okex, Okexfutures, Okexswap
NEOOKB|3|9|Okex, Okexfutures, Okexswap
LTCOKB|3|9|Okex, Okexfutures, Okexswap
ETCOKB|3|9|Okex, Okexfutures, Okexswap
XRPOKB|3|9|Okex, Okexfutures, Okexswap
ZECOKB|3|9|Okex, Okexfutures, Okexswap
IOTAOKB|3|9|Okex, Okexfutures, Okexswap
EOSOKB|3|9|Okex, Okexfutures, Okexswap
OKBUSDC|3|9|Okex, Okexfutures, Okexswap
ETCUSDC|4|16|Okex, Okexfutures, Okexswap, Poloniex
BSVUSDC|4|16|Okex, Okexfutures, Okexswap, Poloniex


This brings a total possible exact matching permutation count of `23,920`.
