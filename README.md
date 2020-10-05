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
The following table is the status as of 5th October 2020.

Exchange | Executium Code |Active | Symbols Count
------------ | ------------ | ------------ | ------------
Binance|binance|Yes|811
Binancefutures|binancefutures|Yes|41
Bitfinex|bitfinex|Yes|314
Bitflyer|bitflyer|Yes|10
Bithumb|bithumb|Yes|111
Bitmart|bitmart|Yes|5
Bitmex|bitmex|Yes|19
Bitstamp|bitstamp|Yes|32
Bittrex|bittrex|Yes|548
Bybit|bybit|Yes|5
Coinbase|coinbase|Yes|169
Coinbasepro|coinbasepro|Yes|97
Coincheck|coincheck|Yes|1
Deribit|deribit|Yes|8
Ftx|ftx|Yes|409
Gateio|gateio|Yes|612
Hbdm|hbdm|Yes|52
Huobipro|huobipro|Yes|751
Indodax|indodax|Yes|68
Itbit|itbit|Yes|6
Kraken|kraken|Yes|155
Krakenfutures|krakenfutures|Yes|17
Kucoin|kucoin|Yes|479
Liquid|liquid|Yes|172
Okex|okex|Yes|481
Okexfutures|okexfutures|Yes|408
Okexswap|okexswap|Yes|408
Poloniex|poloniex|Yes|267
Upbit|upbit|Yes|280
Zb|zb|Yes|177

## Supported Symbols in Version 2
We have increased our symbols and exchange support with version 2, as of the 26th August 2020 (https://executium.com/symbols-exchanges-marketspreads/). 

Version | Exchanges | Markets | Market Spreads | Permutation 
------------ | ------------ | ------------  | ------------   | ------------
Version 2|29|6,269|19,647,046|39,294,092
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

