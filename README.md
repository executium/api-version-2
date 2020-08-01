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
A table of supported exchanges in executium for version 2. The following table is the status as of 1st August 2020.

Exchange | Executium Code |Active | Symbols Count
------------ | ------------ | ------------ | ------------
Binance|binance|Yes|638
Bitfinex|bitfinex|Yes|305
Bitflyer|bitflyer|Yes|10
Bithumb|bithumb|Yes|104
Bitmart|bitmart|Yes|5
Bitmex|bitmex|Yes|15
Bitstamp|bitstamp|Yes|32
Bittrex|bittrex|Yes|484
Bybit|bybit|Yes|5
Coinbase|coinbase|Yes|169
Coinbasepro|coinbasepro|Yes|74
Coincheck|coincheck|Yes|1
Deribit|deribit|Yes|8
Ftx|ftx|Yes|366
Gateio|gateio|Yes|473
Hbdm|hbdm|Yes|44
Huobipro|huobipro|Yes|573
Indodax|indodax|Yes|68
Itbit|itbit|Yes|6
Kraken|kraken|Yes|155
Kucoin|kucoin|Yes|451
Liquid|liquid|Yes|157
Okex|okex|Yes|386
Poloniex|poloniex|Yes|199
Upbit|upbit|Yes|263

## Supported Symbols in Version 2
We have increased our symbols and exchange support with version 2, as of the 1st August 2020 (https://executium.com/symbols-exchanges-marketspreads/). 

Version | Exchanges | Markets | Market Spreads | Permutation 
------------ | ------------ | ------------  | ------------   | ------------
Version 2|25|4,991|12,452,545 | 24,905,090
Version 1|12|138|871 | 871

### Quote to Quote Permutation

Quote | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
BTC|1457|2,122,849|Binance, Bitfinex, Bitflyer, Bitmart, Bittrex, Coinbasepro, Ftx, Kucoin, Liquid, Okex, Poloniex, Upbit
ETH|709|502,681|Binance, Bitfinex, Bittrex, Coinbasepro, Kucoin, Liquid, Okex, Poloniex
USDT|1021|1,042,441|Binance, Bitmart, Bittrex, Bybit, Ftx, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
BNB|85|7,225|Binance, Poloniex
TUSD|17|289|Binance, Kucoin
PAX|18|324|Binance, Bitmart, Kucoin, Poloniex
USDC|67|4,489|Binance, Bitmart, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
TRX|26|676|Binance, Kucoin, Poloniex
BUSD|68|4,624|Binance, Poloniex
NGN|4|16|Binance, Coinbase
RUB|7|49|Binance, Coinbase
TRY|7|49|Binance, Coinbase
EUR|53|2,809|Binance, Bitfinex, Bitflyer, Bittrex, Coinbase, Coinbasepro, Itbit, Liquid
ZAR|6|36|Binance, Coinbase
BKRW|5|25|Binance
IDRT|5|25|Binance, Liquid
GBP|29|841|Binance, Bitfinex, Coinbase, Coinbasepro
UAH|3|9|Binance, Coinbase
BIDR|5|25|Binance
AUD|6|36|Binance, Coinbase, Liquid
USD|552|304,704|Bitfinex, Bitflyer, Bittrex, Bybit, Coinbase, Coinbasepro, Deribit, Ftx, Itbit, Liquid
JPY|20|400|Bitfinex, Bitflyer, Coinbase, Liquid
EOS|3|9|Bitfinex
DAI|14|196|Bitfinex, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
UST|20|400|Bitfinex
CNHT|3|9|Bitfinex
USTF0|5|25|Bitfinex
KRW|198|39,204|Bithumb, Coinbase, Upbit
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
QASH|14|196|Liquid
USDK|31|961|Okex
OKB|12|144|Okex
USDJ|3|9|Poloniex


### Base to Base Permutation

Base | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
ETH|97|9,409|Binance, Bitfinex, Bitflyer, Bithumb, Bitmart, Bitmex, Bittrex, Bybit, Coinbasepro, Deribit, Ftx, Hbdm, Itbit, Kucoin, Liquid, Okex, Poloniex, Upbit
LTC|59|3,481|Binance, Bitfinex, Bithumb, Bitmex, Bittrex, Coinbasepro, Ftx, Hbdm, Kucoin, Liquid, Okex, Poloniex, Upbit
BNB|27|729|Binance, Ftx, Kucoin, Poloniex
NEO|32|1,024|Binance, Bitfinex, Bittrex, Kucoin, Okex, Poloniex, Upbit
QTUM|26|676|Binance, Bithumb, Bittrex, Kraken, Kucoin, Okex, Poloniex, Upbit
EOS|60|3,600|Binance, Bitfinex, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hbdm, Kraken, Kucoin, Okex, Poloniex, Upbit
SNT|20|400|Binance, Bitfinex, Bithumb, Bittrex, Kucoin, Okex, Poloniex, Upbit
BTC|266|70,756|Binance, Bitfinex, Bitflyer, Bithumb, Bitmart, Bittrex, Bybit, Coinbase, Coinbasepro, Deribit, Ftx, Hbdm, Kucoin, Liquid, Okex, Poloniex, Upbit
OMG|34|1,156|Binance, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
ZRX|33|1,089|Binance, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kucoin, Okex, Poloniex, Upbit
KNC|24|576|Binance, Bitfinex, Bithumb, Coinbasepro, Ftx, Kucoin, Okex, Poloniex, Upbit
LINK|40|1,600|Binance, Bithumb, Bittrex, Coinbasepro, Ftx, Hbdm, Kraken, Okex, Poloniex, Upbit
ETC|46|2,116|Binance, Bitfinex, Bithumb, Bittrex, Coinbasepro, Ftx, Hbdm, Kucoin, Okex, Poloniex, Upbit
ZEC|31|961|Binance, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kucoin, Okex, Poloniex
DASH|32|1,024|Binance, Bithumb, Bittrex, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
TRX|57|3,249|Binance, Bitfinex, Bithumb, Bitmex, Bittrex, Ftx, Hbdm, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
XRP|74|5,476|Binance, Bitfinex, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hbdm, Kucoin, Liquid, Okex, Poloniex, Upbit
XMR|24|576|Binance, Bitfinex, Bittrex, Kucoin, Okex, Poloniex
BAT|35|1,225|Binance, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kraken, Okex, Poloniex, Upbit
LSK|20|400|Binance, Bittrex, Kraken, Kucoin, Okex, Poloniex, Upbit
MANA|20|400|Binance, Bittrex, Coinbasepro, Kucoin, Okex, Poloniex, Upbit
ADA|39|1,521|Binance, Bithumb, Bitmex, Bittrex, Ftx, Hbdm, Kraken, Kucoin, Okex, Upbit
XLM|37|1,369|Binance, Bitfinex, Bithumb, Bittrex, Coinbasepro, Kucoin, Okex, Upbit
WAVES|25|625|Binance, Bithumb, Bittrex, Kraken, Kucoin, Okex, Upbit
ZIL|20|400|Binance, Bitfinex, Bithumb, Bittrex, Kucoin, Okex, Upbit
ONT|20|400|Binance, Bittrex, Kucoin, Okex, Upbit
GNT|20|400|Binance, Bitfinex, Bithumb, Bittrex, Coinbasepro, Okex, Poloniex, Upbit
SC|23|529|Binance, Bittrex, Kraken, Okex, Poloniex, Upbit
VET|22|484|Binance, Bitfinex, Bithumb, Bittrex, Ftx, Kucoin, Upbit
BCH|56|3,136|Binance, Bitflyer, Bithumb, Bitmex, Bittrex, Coinbasepro, Ftx, Hbdm, Kraken, Liquid, Okex, Upbit
BTT|31|961|Binance, Bitfinex, Bithumb, Bittrex, Kucoin, Okex, Poloniex, Upbit
ATOM|34|1,156|Binance, Bittrex, Coinbasepro, Ftx, Kraken, Kucoin, Okex, Poloniex, Upbit
ALGO|29|841|Binance, Bithumb, Bittrex, Coinbasepro, Ftx, Kraken, Kucoin, Okex
DOGE|23|529|Binance, Bittrex, Ftx, Okex, Poloniex, Upbit
XTZ|34|1,156|Binance, Bitfinex, Bittrex, Coinbasepro, Ftx, Kraken, Kucoin, Okex, Poloniex, Upbit
USDT|26|676|Binance, Bittrex, Ftx, Kraken, Kucoin, Okex, Poloniex
COMP|20|400|Binance, Bittrex, Coinbasepro, Ftx, Kucoin, Okex, Poloniex
MKR|25|625|Binance, Bitfinex, Coinbasepro, Ftx, Kucoin, Okex, Poloniex, Upbit
DAI|20|400|Binance, Bitfinex, Bittrex, Coinbasepro, Kraken, Okex, Poloniex, Upbit
BSV|23|529|Bitfinex, Bithumb, Bittrex, Ftx, Hbdm, Okex, Upbit


### Pairing Permutation (Exact symbol match)

Base | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
ETHBTC|17|289|Binance, Bitfinex, Bitflyer, Bitmart, Bitstamp, Bittrex, Coinbasepro, Ftx, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
LTCBTC|14|196|Binance, Bitfinex, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
BNBBTC|2|4|Binance, Kucoin
NEOBTC|8|64|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
QTUMETH|6|36|Binance, Bittrex, Gateio, Huobipro, Kraken, Okex
EOSETH|9|81|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex
SNTETH|5|25|Binance, Bitfinex, Bittrex, Gateio, Kucoin
BNTETH|3|9|Binance, Bittrex, Gateio
GASBTC|6|36|Binance, Gateio, Huobipro, Kucoin, Okex, Poloniex
BTCUSDT|14|196|Binance, Bitfinex, Bitmart, Bittrex, Bybit, Ftx, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
ETHUSDT|13|169|Binance, Bitfinex, Bitmart, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
MCOETH|5|25|Binance, Bittrex, Gateio, Huobipro, Okex
MCOBTC|5|25|Binance, Bittrex, Huobipro, Okex, Upbit
WTCBTC|4|16|Binance, Huobipro, Kucoin, Okex
WTCETH|3|9|Binance, Huobipro, Okex
LRCBTC|7|49|Binance, Bitfinex, Bittrex, Gateio, Okex, Poloniex, Upbit
LRCETH|3|9|Binance, Gateio, Okex
QTUMBTC|10|100|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
YOYOWBTC|2|4|Binance, Okex
OMGBTC|12|144|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
OMGETH|8|64|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex
ZRXBTC|10|100|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
ZRXETH|8|64|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
STRATBTC|4|16|Binance, Bittrex, Poloniex, Upbit
STRATETH|2|4|Binance, Bittrex
KNCBTC|7|49|Binance, Bitfinex, Coinbasepro, Huobipro, Kucoin, Okex, Poloniex
KNCETH|4|16|Binance, Gateio, Huobipro, Kucoin
FUNBTC|2|4|Binance, Okex
FUNETH|3|9|Binance, Bitfinex, Gateio
NEOETH|5|25|Binance, Bitfinex, Bittrex, Kucoin, Okex
IOTABTC|6|36|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Okex
IOTAETH|4|16|Binance, Bitfinex, Huobipro, Okex
LINKBTC|7|49|Binance, Bittrex, Huobipro, Kraken, Okex, Poloniex, Upbit
LINKETH|7|49|Binance, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Okex
XVGBTC|5|25|Binance, Bitfinex, Bittrex, Gateio, Huobipro
XVGETH|2|4|Binance, Huobipro
MTLBTC|4|16|Binance, Bittrex, Huobipro, Upbit
EOSBTC|11|121|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
SNTBTC|9|81|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
ETCETH|7|49|Binance, Bittrex, Gateio, Kraken, Kucoin, Okex, Poloniex
ETCBTC|11|121|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
ENGBTC|4|16|Binance, Bittrex, Huobipro, Upbit
ENGETH|2|4|Binance, Bittrex
DNTBTC|3|9|Binance, Bittrex, Upbit
ZECBTC|10|100|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex
ZECETH|4|16|Binance, Bittrex, Okex, Poloniex
BNTBTC|5|25|Binance, Bittrex, Okex, Poloniex, Upbit
ASTBTC|2|4|Binance, Huobipro
DASHBTC|12|144|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Poloniex
DASHETH|4|16|Binance, Bittrex, Kucoin, Okex
OAXBTC|2|4|Binance, Gateio
BTGBTC|5|25|Binance, Bitfinex, Gateio, Huobipro, Okex
EVXBTC|2|4|Binance, Huobipro
EVXETH|2|4|Binance, Huobipro
REQBTC|3|9|Binance, Huobipro, Kucoin
VIBBTC|4|16|Binance, Bittrex, Okex, Upbit
VIBETH|2|4|Binance, Bittrex
TRXBTC|10|100|Binance, Bitfinex, Bittrex, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
TRXETH|8|64|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex
POWRBTC|6|36|Binance, Bittrex, Gateio, Huobipro, Kucoin, Upbit
POWRETH|5|25|Binance, Bittrex, Gateio, Huobipro, Kucoin
ARKBTC|4|16|Binance, Bittrex, Okex, Upbit
XRPBTC|14|196|Binance, Bitfinex, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
XRPETH|5|25|Binance, Bittrex, Kraken, Kucoin, Okex
ENJBTC|4|16|Binance, Bittrex, Kucoin, Upbit
ENJETH|3|9|Binance, Bittrex, Kucoin
STORJBTC|6|36|Binance, Bittrex, Gateio, Huobipro, Poloniex, Upbit
STORJETH|3|9|Binance, Gateio, Okex
BNBUSDT|5|25|Binance, Ftx, Gateio, Kucoin, Poloniex
KMDBTC|5|25|Binance, Bittrex, Huobipro, Liquid, Upbit
KMDETH|2|4|Binance, Huobipro
RCNBTC|4|16|Binance, Bittrex, Huobipro, Upbit
NULSBTC|4|16|Binance, Huobipro, Kucoin, Okex
NULSETH|4|16|Binance, Huobipro, Kucoin, Okex
RDNBTC|2|4|Binance, Huobipro
XMRBTC|9|81|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex
XMRETH|5|25|Binance, Bittrex, Huobipro, Kucoin, Okex
AMBBTC|2|4|Binance, Kucoin
BATBTC|9|81|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kraken, Okex, Poloniex, Upbit
BATETH|8|64|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Poloniex
BCPTBTC|2|4|Binance, Upbit
CDTETH|2|4|Binance, Gateio
GXSBTC|2|4|Binance, Gateio
NEOUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
QSPBTC|2|4|Binance, Huobipro
QSPETH|2|4|Binance, Gateio
BTSBTC|7|49|Binance, Bittrex, Gateio, Huobipro, Indodax, Poloniex, Upbit
XZCBTC|3|9|Binance, Bittrex, Huobipro
XZCETH|2|4|Binance, Huobipro
LSKBTC|9|81|Binance, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
LSKETH|4|16|Binance, Huobipro, Kraken, Kucoin
TNTETH|2|4|Binance, Gateio
MANABTC|8|64|Binance, Bitfinex, Bittrex, Huobipro, Kucoin, Okex, Poloniex, Upbit
MANAETH|6|36|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex
BCDBTC|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
ADXBTC|4|16|Binance, Bittrex, Huobipro, Upbit
ADXETH|2|4|Binance, Bittrex
ADABTC|8|64|Binance, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Upbit
ADAETH|5|25|Binance, Bittrex, Huobipro, Kraken, Okex
PPTBTC|2|4|Binance, Kucoin
CMTBTC|3|9|Binance, Huobipro, Okex
CMTETH|3|9|Binance, Huobipro, Okex
XLMBTC|13|169|Binance, Bitfinex, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Indodax, Kraken, Kucoin, Okex, Poloniex, Upbit
XLMETH|7|49|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex
CNDBTC|2|4|Binance, Bittrex
LENDBTC|2|4|Binance, Poloniex
LENDETH|2|4|Binance, Gateio
WABIBTC|2|4|Binance, Liquid
LTCETH|5|25|Binance, Bittrex, Kraken, Kucoin, Okex
LTCUSDT|11|121|Binance, Bitfinex, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
TNBBTC|3|9|Binance, Bitfinex, Huobipro
WAVESBTC|8|64|Binance, Bittrex, Gateio, Huobipro, Kraken, Kucoin, Okex, Upbit
WAVESETH|5|25|Binance, Bittrex, Huobipro, Kraken, Okex
GTOBTC|4|16|Binance, Bittrex, Okex, Upbit
ICXBTC|5|25|Binance, Bittrex, Huobipro, Kraken, Okex
ICXETH|4|16|Binance, Gateio, Huobipro, Kraken
OSTBTC|4|16|Binance, Bittrex, Huobipro, Upbit
OSTETH|2|4|Binance, Gateio
ELFBTC|6|36|Binance, Bittrex, Huobipro, Kucoin, Okex, Upbit
ELFETH|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
AIONBTC|3|9|Binance, Bitfinex, Kucoin
AIONETH|2|4|Binance, Kucoin
NEBLBTC|2|4|Binance, Kucoin
NAVBTC|2|4|Binance, Bittrex
APPCBTC|2|4|Binance, Huobipro
RLCBTC|4|16|Binance, Bitfinex, Bittrex, Upbit
RLCETH|2|4|Binance, Gateio
PIVXBTC|3|9|Binance, Bittrex, Kucoin
PIVXETH|2|4|Binance, Kucoin
IOSTBTC|7|49|Binance, Bitfinex, Bittrex, Huobipro, Kucoin, Okex, Upbit
IOSTETH|5|25|Binance, Bitfinex, Huobipro, Kucoin, Okex
STEEMBTC|5|25|Binance, Bittrex, Huobipro, Poloniex, Upbit
STEEMETH|2|4|Binance, Huobipro
NANOBTC|6|36|Binance, Gateio, Huobipro, Kraken, Kucoin, Okex
NANOETH|5|25|Binance, Huobipro, Kraken, Kucoin, Okex
VIABTC|2|4|Binance, Bittrex
BLZBTC|2|4|Binance, Huobipro
BLZETH|3|9|Binance, Gateio, Huobipro
AEBTC|3|9|Binance, Gateio, Huobipro
AEETH|3|9|Binance, Gateio, Huobipro
ZILBTC|6|36|Binance, Bittrex, Huobipro, Kucoin, Okex, Upbit
ZILETH|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
ONTBTC|5|25|Binance, Bittrex, Huobipro, Kucoin, Okex
ONTETH|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
QTUMUSDT|5|25|Binance, Gateio, Huobipro, Okex, Poloniex
XEMBTC|10|100|Binance, Bittrex, Gateio, Huobipro, Indodax, Kucoin, Liquid, Okex, Poloniex, Upbit
XEMETH|4|16|Binance, Bittrex, Gateio, Okex
WANBTC|3|9|Binance, Huobipro, Kucoin
WANETH|3|9|Binance, Huobipro, Kucoin
WPRBTC|2|4|Binance, Huobipro
QLCBTC|2|4|Binance, Gateio
QLCETH|2|4|Binance, Gateio
SYSBTC|3|9|Binance, Bittrex, Upbit
GRSBTC|4|16|Binance, Bittrex, Huobipro, Upbit
ADAUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Upbit
GNTBTC|7|49|Binance, Bitfinex, Bittrex, Huobipro, Okex, Poloniex, Upbit
GNTETH|5|25|Binance, Bitfinex, Bittrex, Gateio, Huobipro
LOOMBTC|6|36|Binance, Bittrex, Huobipro, Kucoin, Poloniex, Upbit
LOOMETH|3|9|Binance, Huobipro, Kucoin
XRPUSDT|10|100|Binance, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
REPBTC|7|49|Binance, Bitfinex, Bittrex, Coinbasepro, Kraken, Poloniex, Upbit
REPETH|5|25|Binance, Bitfinex, Bittrex, Gateio, Kraken
BTCTUSD|2|4|Binance, Kucoin
ETHTUSD|2|4|Binance, Kucoin
ZENBTC|4|16|Binance, Bittrex, Huobipro, Okex
ZENETH|3|9|Binance, Huobipro, Okex
EOSUSDT|8|64|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
CVCBTC|7|49|Binance, Bittrex, Huobipro, Kucoin, Okex, Poloniex, Upbit
CVCETH|5|25|Binance, Bittrex, Gateio, Huobipro, Okex
THETABTC|3|9|Binance, Huobipro, Okex
THETAETH|3|9|Binance, Gateio, Huobipro
TUSDUSDT|6|36|Binance, Bitfinex, Bittrex, Gateio, Okex, Upbit
IOTAUSDT|4|16|Binance, Gateio, Huobipro, Okex
XLMUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
IOTXBTC|4|16|Binance, Bittrex, Kucoin, Upbit
IOTXETH|3|9|Binance, Gateio, Kucoin
QKCBTC|3|9|Binance, Gateio, Kucoin
QKCETH|3|9|Binance, Gateio, Kucoin
AGIBTC|2|4|Binance, Kucoin
NXSBTC|3|9|Binance, Bittrex, Upbit
DATABTC|2|4|Binance, Bitfinex
DATAETH|3|9|Binance, Bitfinex, Gateio
ONTUSDT|6|36|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex
TRXUSDT|9|81|Binance, Bittrex, Ftx, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
ETCUSDT|8|64|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
ICXUSDT|3|9|Binance, Gateio, Okex
SCBTC|7|49|Binance, Bittrex, Huobipro, Kraken, Okex, Poloniex, Upbit
SCETH|5|25|Binance, Bittrex, Huobipro, Kraken, Okex
NPXSETH|4|16|Binance, Bittrex, Huobipro, Kucoin
KEYETH|2|4|Binance, Kucoin
NASBTC|4|16|Binance, Gateio, Huobipro, Okex
NASETH|4|16|Binance, Gateio, Huobipro, Okex
DENTETH|2|4|Binance, Kucoin
ARDRBTC|6|36|Binance, Bittrex, Huobipro, Okex, Poloniex, Upbit
NULSUSDT|3|9|Binance, Huobipro, Okex
VETBTC|6|36|Binance, Bitfinex, Bittrex, Huobipro, Kucoin, Upbit
VETETH|4|16|Binance, Gateio, Huobipro, Kucoin
VETUSDT|5|25|Binance, Bittrex, Gateio, Huobipro, Kucoin
DOCKBTC|3|9|Binance, Huobipro, Kucoin
POLYBTC|4|16|Binance, Huobipro, Poloniex, Upbit
HCBTC|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
GOBTC|4|16|Binance, Bittrex, Kucoin, Upbit
PAXUSDT|5|25|Binance, Bitfinex, Gateio, Okex, Poloniex
RVNBTC|5|25|Binance, Bittrex, Huobipro, Okex, Upbit
DCRBTC|8|64|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
MITHBTC|2|4|Binance, Okex
BCHBTC|14|196|Binance, Bitfinex, Bitflyer, Bitstamp, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Liquid, Okex, Poloniex, Upbit
BCHUSDT|11|121|Binance, Bitfinex, Bittrex, Ftx, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
BTCPAX|6|36|Binance, Bitmart, Bitstamp, Gateio, Kucoin, Poloniex
ETHPAX|4|16|Binance, Bitstamp, Kucoin, Poloniex
XRPPAX|3|9|Binance, Bitstamp, Kucoin
RENBTC|3|9|Binance, Huobipro, Poloniex
XRPTUSD|2|4|Binance, Kucoin
BTCUSDC|9|81|Binance, Bitmart, Coinbasepro, Gateio, Kraken, Kucoin, Liquid, Okex, Poloniex
ETHUSDC|7|49|Binance, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
XRPUSDC|3|9|Binance, Okex, Poloniex
EOSUSDC|3|9|Binance, Okex, Poloniex
USDCUSDT|6|36|Binance, Bitfinex, Bittrex, Gateio, Kraken, Okex
LINKUSDT|7|49|Binance, Bittrex, Ftx, Gateio, Huobipro, Okex, Poloniex
WAVESUSDT|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
BCHUSDC|4|16|Binance, Liquid, Okex, Poloniex
LTCUSDC|3|9|Binance, Okex, Poloniex
TRXUSDC|3|9|Binance, Okex, Poloniex
BTTUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
ONGBTC|2|4|Binance, Bittrex
ONGUSDT|2|4|Binance, Gateio
ZILUSDT|4|16|Binance, Gateio, Huobipro, Okex
ZRXUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Okex, Poloniex, Upbit
FETBTC|2|4|Binance, Kucoin
BATUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Okex, Poloniex, Upbit
XMRUSDT|6|36|Binance, Bittrex, Gateio, Huobipro, Okex, Poloniex
ZECUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
ZECUSDC|3|9|Binance, Coinbasepro, Poloniex
IOSTUSDT|3|9|Binance, Huobipro, Okex
CELRUSDT|2|4|Binance, Gateio
DASHUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
NANOUSDT|5|25|Binance, Gateio, Huobipro, Kucoin, Okex
OMGUSDT|6|36|Binance, Bittrex, Gateio, Huobipro, Okex, Upbit
THETAUSDT|4|16|Binance, Gateio, Huobipro, Okex
ENJUSDT|2|4|Binance, Bittrex
MITHUSDT|3|9|Binance, Gateio, Okex
MATICBTC|2|4|Binance, Poloniex
MATICUSDT|2|4|Binance, Poloniex
ATOMBTC|11|121|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
ATOMUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
ATOMUSDC|2|4|Binance, Poloniex
BATUSDC|2|4|Binance, Coinbasepro
TFUELUSDT|2|4|Binance, Gateio
ONEBTC|3|9|Binance, Huobipro, Kucoin
ONEUSDT|4|16|Binance, Gateio, Huobipro, Kucoin
FTMBTC|2|4|Binance, Kucoin
FTMUSDT|3|9|Binance, Gateio, Okex
ALGOBTC|7|49|Binance, Bitfinex, Bittrex, Huobipro, Kraken, Kucoin, Okex
ALGOUSDT|7|49|Binance, Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex
GTOUSDT|2|4|Binance, Okex
DOGEBTC|8|64|Binance, Bittrex, Gateio, Huobipro, Indodax, Kraken, Poloniex, Upbit
DOGEUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Okex, Poloniex, Upbit
DUSKBTC|3|9|Binance, Bitfinex, Bittrex
ANKRBTC|4|16|Binance, Bittrex, Kucoin, Upbit
ANKRUSDT|2|4|Binance, Gateio
WINUSDT|4|16|Binance, Gateio, Kucoin, Poloniex
COSUSDT|2|4|Binance, Gateio
NPXSUSDT|2|4|Binance, Bittrex
TOMOBTC|2|4|Binance, Kucoin
TOMOUSDT|3|9|Binance, Gateio, Kucoin
DOCKUSDT|3|9|Binance, Gateio, Huobipro
FUNUSDT|2|4|Binance, Gateio
CVCUSDT|4|16|Binance, Gateio, Huobipro, Okex
BTTTRX|5|25|Binance, Gateio, Huobipro, Kucoin, Poloniex
WINTRX|3|9|Binance, Kucoin, Poloniex
CHZBTC|3|9|Binance, Kucoin, Upbit
CHZUSDT|2|4|Binance, Bitfinex
BNBBUSD|2|4|Binance, Poloniex
BTCBUSD|2|4|Binance, Poloniex
BUSDUSDT|2|4|Binance, Poloniex
BEAMBTC|2|4|Binance, Gateio
BEAMUSDT|2|4|Binance, Gateio
XTZBTC|11|121|Binance, Bitfinex, Bittrex, Coinbasepro, Gateio, Huobipro, Kraken, Kucoin, Okex, Poloniex, Upbit
XTZUSDT|7|49|Binance, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
RENUSDT|3|9|Binance, Huobipro, Poloniex
RVNUSDT|6|36|Binance, Bittrex, Gateio, Huobipro, Okex, Upbit
HCUSDT|4|16|Binance, Gateio, Huobipro, Okex
HBARBTC|4|16|Binance, Bittrex, Liquid, Okex
HBARUSDT|4|16|Binance, Bittrex, Gateio, Okex
NKNBTC|4|16|Binance, Bittrex, Huobipro, Upbit
NKNUSDT|3|9|Binance, Gateio, Huobipro
STXBTC|2|4|Binance, Kucoin
STXUSDT|3|9|Binance, Gateio, Kucoin
KAVABTC|2|4|Binance, Upbit
KAVAUSDT|2|4|Binance, Gateio
BTCNGN|2|4|Binance, Coinbase
ARPABTC|2|4|Binance, Huobipro
ARPAUSDT|4|16|Binance, Gateio, Huobipro, Kucoin
IOTXUSDT|2|4|Binance, Gateio
RLCUSDT|2|4|Binance, Gateio
MCOUSDT|4|16|Binance, Gateio, Huobipro, Okex
CTXCBTC|5|25|Binance, Bittrex, Huobipro, Okex, Upbit
CTXCUSDT|3|9|Binance, Huobipro, Okex
BTCRUB|2|4|Binance, Coinbase
VITEBTC|4|16|Binance, Bittrex, Okex, Upbit
FTTBTC|3|9|Binance, Ftx, Huobipro
FTTUSDT|4|16|Binance, Bitfinex, Ftx, Huobipro
BTCTRY|2|4|Binance, Coinbase
BTCEUR|10|100|Binance, Bitfinex, Bitflyer, Bitstamp, Bittrex, Coinbase, Coinbasepro, Itbit, Kraken, Liquid
ETHEUR|8|64|Binance, Bitfinex, Bitstamp, Bittrex, Coinbasepro, Itbit, Kraken, Liquid
XRPEUR|5|25|Binance, Bitstamp, Coinbasepro, Kraken, Liquid
OGNBTC|4|16|Binance, Bittrex, Huobipro, Upbit
OGNUSDT|2|4|Binance, Huobipro
DREPUSDT|2|4|Binance, Gateio
TCTBTC|2|4|Binance, Okex
TCTUSDT|3|9|Binance, Gateio, Okex
WRXBTC|2|4|Binance, Poloniex
WRXUSDT|3|9|Binance, Ftx, Poloniex
BTSUSDT|3|9|Binance, Gateio, Huobipro
LSKUSDT|4|16|Binance, Gateio, Okex, Poloniex
BNTUSDT|2|4|Binance, Okex
MBLUSDT|2|4|Binance, Gateio
COTIBTC|2|4|Binance, Kucoin
COTIUSDT|3|9|Binance, Gateio, Kucoin
STPTBTC|4|16|Binance, Bittrex, Poloniex, Upbit
STPTUSDT|2|4|Binance, Poloniex
BTCZAR|2|4|Binance, Coinbase
WTCUSDT|3|9|Binance, Huobipro, Okex
DATAUSDT|2|4|Binance, Gateio
XZCUSDT|2|4|Binance, Huobipro
SOLBTC|2|4|Binance, Ftx
BTCIDRT|2|4|Binance, Liquid
CTSIUSDT|2|4|Binance, Gateio
HIVEBTC|4|16|Binance, Bittrex, Huobipro, Upbit
HIVEUSDT|4|16|Binance, Bittrex, Gateio, Huobipro
CHRBTC|5|25|Binance, Bittrex, Huobipro, Kucoin, Poloniex
CHRUSDT|4|16|Binance, Huobipro, Kucoin, Poloniex
GXSUSDT|2|4|Binance, Gateio
LENDUSDT|3|9|Binance, Gateio, Poloniex
MDTBTC|5|25|Binance, Bittrex, Gateio, Okex, Poloniex
MDTUSDT|5|25|Binance, Bittrex, Gateio, Okex, Poloniex
STMXBTC|3|9|Binance, Bittrex, Upbit
STMXETH|2|4|Binance, Bittrex
KNCUSDT|5|25|Binance, Ftx, Gateio, Huobipro, Okex
REPUSDT|2|4|Binance, Poloniex
LRCUSDT|4|16|Binance, Gateio, Okex, Poloniex
PNTBTC|2|4|Binance, Huobipro
BTCGBP|6|36|Binance, Bitfinex, Bitstamp, Coinbase, Coinbasepro, Kraken
ETHGBP|5|25|Binance, Bitfinex, Bitstamp, Coinbasepro, Kraken
XRPGBP|4|16|Binance, Bitstamp, Coinbasepro, Kraken
DGBBTC|7|49|Binance, Bitfinex, Bittrex, Huobipro, Kucoin, Okex, Upbit
BTCUAH|2|4|Binance, Coinbase
COMPBTC|4|16|Binance, Bittrex, Coinbasepro, Okex
COMPUSDT|7|49|Binance, Bittrex, Ftx, Gateio, Kucoin, Okex, Poloniex
SCUSDT|5|25|Binance, Bittrex, Okex, Poloniex, Upbit
ZENUSDT|2|4|Binance, Okex
SXPBTC|4|16|Binance, Bittrex, Kucoin, Poloniex
SNXBTC|3|9|Binance, Kucoin, Poloniex
SNXUSDT|4|16|Binance, Kucoin, Okex, Poloniex
VTHOUSDT|2|4|Binance, Gateio
DGBUSDT|5|25|Binance, Bittrex, Kucoin, Okex, Upbit
SXPUSDT|4|16|Binance, Ftx, Kucoin, Poloniex
IRISBTC|3|9|Binance, Bittrex, Huobipro
MKRBTC|7|49|Binance, Bitfinex, Coinbasepro, Kucoin, Okex, Poloniex, Upbit
MKRUSDT|5|25|Binance, Ftx, Gateio, Okex, Poloniex
DAIBTC|4|16|Binance, Bitfinex, Bittrex, Upbit
DAIUSDT|6|36|Binance, Bittrex, Gateio, Kraken, Okex, Poloniex
DCRUSDT|6|36|Binance, Bittrex, Gateio, Huobipro, Okex, Upbit
STORJUSDT|4|16|Binance, Gateio, Huobipro, Okex
BTCAUD|3|9|Binance, Coinbase, Liquid
ETHAUD|2|4|Binance, Liquid
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
TNBETH|2|4|Bitfinex, Huobipro
TRXUSD|4|16|Bitfinex, Bittrex, Ftx, Kraken
REPUSD|3|9|Bitfinex, Coinbasepro, Kraken
ETHJPY|4|16|Bitfinex, Bitflyer, Kraken, Liquid
EOSEUR|3|9|Bitfinex, Coinbasepro, Kraken
WAXPUSD|2|4|Bitfinex, Bittrex
WAXPBTC|5|25|Bitfinex, Bittrex, Huobipro, Kucoin, Upbit
DAIUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
DAIETH|2|4|Bitfinex, Bittrex
BFTBTC|4|16|Bitfinex, Bittrex, Huobipro, Upbit
ANTBTC|3|9|Bitfinex, Bittrex, Upbit
ANTETH|2|4|Bitfinex, Bittrex
XLMUSD|5|25|Bitfinex, Bitstamp, Bittrex, Coinbasepro, Kraken
XLMEUR|4|16|Bitfinex, Bitstamp, Coinbasepro, Kraken
XLMGBP|2|4|Bitfinex, Bitstamp
MKRUSD|3|9|Bitfinex, Coinbasepro, Ftx
MKRETH|4|16|Bitfinex, Gateio, Kucoin, Okex
KNCUSD|3|9|Bitfinex, Coinbasepro, Ftx
XTZUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
TRXEUR|3|9|Bitfinex, Bittrex, Kraken
MLNUSD|2|4|Bitfinex, Kraken
DGBUSD|2|4|Bitfinex, Bittrex
BSVUSD|2|4|Bitfinex, Bittrex
BSVBTC|8|64|Bitfinex, Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex, Upbit
BCHUSD|8|64|Bitfinex, Bitmex, Bitstamp, Bittrex, Coinbasepro, Ftx, Kraken, Liquid
ENJUSD|2|4|Bitfinex, Bittrex
USDTUSD|4|16|Bitfinex, Bittrex, Ftx, Kraken
USDCUSD|3|9|Bitfinex, Bittrex, Kraken
TUSDUSD|2|4|Bitfinex, Bittrex
PAXUSD|3|9|Bitfinex, Bitstamp, Bittrex
RIFUSD|2|4|Bitfinex, Liquid
RIFBTC|3|9|Bitfinex, Kucoin, Liquid
VSYSBTC|4|16|Bitfinex, Huobipro, Kucoin, Okex
MKRDAI|2|4|Bitfinex, Kucoin
BTTBTC|6|36|Bitfinex, Bittrex, Huobipro, Kucoin, Okex, Upbit
GNOUSD|2|4|Bitfinex, Kraken
ATOMUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
ATOMETH|6|36|Bitfinex, Bittrex, Huobipro, Kraken, Kucoin, Okex
LEOBTC|3|9|Bitfinex, Gateio, Okex
LEOUSDT|3|9|Bitfinex, Gateio, Okex
LEOETH|2|4|Bitfinex, Okex
OKBUSDT|3|9|Bitfinex, Gateio, Okex
OKBBTC|2|4|Bitfinex, Okex
KANUSDT|3|9|Bitfinex, Huobipro, Okex
AMPLUSD|2|4|Bitfinex, Ftx
ALGOUSD|4|16|Bitfinex, Bittrex, Coinbasepro, Kraken
AMPLUSDT|4|16|Bitfinex, Ftx, Gateio, Kucoin
AMPLBTC|2|4|Bitfinex, Kucoin
FTTUSD|2|4|Bitfinex, Ftx
XAUTUSD|2|4|Bitfinex, Ftx
XAUTUSDT|2|4|Bitfinex, Ftx
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
MCOKRW|2|4|Bithumb, Upbit
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
ENJKRW|2|4|Bithumb, Upbit
VETKRW|2|4|Bithumb, Upbit
MTLKRW|2|4|Bithumb, Upbit
IOSTKRW|2|4|Bithumb, Upbit
QKCKRW|2|4|Bithumb, Upbit
NPXSKRW|2|4|Bithumb, Upbit
BSVKRW|2|4|Bithumb, Upbit
ORBSKRW|2|4|Bithumb, Upbit
ANKRKRW|2|4|Bithumb, Upbit
MBLKRW|2|4|Bithumb, Upbit
XLMKRW|2|4|Bithumb, Upbit
BTTKRW|2|4|Bithumb, Upbit
GBPUSD|2|4|Bitstamp, Kraken
EURUSD|2|4|Bitstamp, Kraken
LTCEUR|3|9|Bitstamp, Coinbasepro, Kraken
LTCGBP|3|9|Bitstamp, Coinbasepro, Kraken
BCHEUR|4|16|Bitstamp, Bittrex, Coinbasepro, Kraken
BCHGBP|3|9|Bitstamp, Coinbasepro, Kraken
ADAUSD|2|4|Bittrex, Kraken
AKROBTC|3|9|Bittrex, Huobipro, Kucoin
APIXBTC|2|4|Bittrex, Okex
APMBTC|2|4|Bittrex, Okex
APMUSDT|2|4|Bittrex, Okex
BCHETH|3|9|Bittrex, Kraken, Kucoin
BLKBTC|2|4|Bittrex, Upbit
BLOCKBTC|2|4|Bittrex, Upbit
BORABTC|2|4|Bittrex, Upbit
BSVETH|2|4|Bittrex, Kucoin
BSVUSDT|6|36|Bittrex, Gateio, Huobipro, Kucoin, Okex, Poloniex
BTMBTC|6|36|Bittrex, Gateio, Huobipro, Kucoin, Okex, Upbit
BTUBTC|2|4|Bittrex, Upbit
BURSTBTC|2|4|Bittrex, Upbit
CELOBTC|2|4|Bittrex, Okex
CELOUSDT|2|4|Bittrex, Okex
CKBBTC|3|9|Bittrex, Gateio, Huobipro
CKBUSDT|3|9|Bittrex, Gateio, Huobipro
CMCTBTC|2|4|Bittrex, Upbit
COMPETH|2|4|Bittrex, Poloniex
COMPUSD|3|9|Bittrex, Coinbasepro, Ftx
CPCBTC|2|4|Bittrex, Kucoin
CROBTC|5|25|Bittrex, Huobipro, Kucoin, Okex, Upbit
CROUSDT|5|25|Bittrex, Gateio, Huobipro, Kucoin, Okex
CRWBTC|2|4|Bittrex, Upbit
CTCBTC|2|4|Bittrex, Okex
CVTBTC|2|4|Bittrex, Okex
DENTBTC|3|9|Bittrex, Kucoin, Upbit
DEPUSDT|2|4|Bittrex, Okex
DGBETH|3|9|Bittrex, Huobipro, Kucoin
DMTBTC|2|4|Bittrex, Upbit
DNABTC|2|4|Bittrex, Okex
DNAUSDT|2|4|Bittrex, Okex
DOGEETH|2|4|Bittrex, Huobipro
DOGEUSD|2|4|Bittrex, Kraken
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
HDAOUSDT|2|4|Bittrex, Okex
HNSBTC|2|4|Bittrex, Gateio
HNSUSDT|2|4|Bittrex, Gateio
HYCBTC|2|4|Bittrex, Okex
IGNISBTC|2|4|Bittrex, Upbit
IRISUSDT|2|4|Bittrex, Huobipro
JNTBTC|3|9|Bittrex, Gateio, Upbit
LAMBBTC|3|9|Bittrex, Huobipro, Upbit
LBABTC|4|16|Bittrex, Huobipro, Okex, Upbit
LBCBTC|2|4|Bittrex, Upbit
LINKUSD|4|16|Bittrex, Coinbasepro, Ftx, Kraken
LUNABTC|4|16|Bittrex, Huobipro, Kucoin, Upbit
LUNAUSDT|3|9|Bittrex, Huobipro, Kucoin
MEDBTC|2|4|Bittrex, Upbit
METABTC|3|9|Bittrex, Kucoin, Upbit
METBTC|2|4|Bittrex, Upbit
METETH|2|4|Bittrex, Gateio
MFTBTC|2|4|Bittrex, Upbit
MOCBTC|2|4|Bittrex, Upbit
MOFBTC|2|4|Bittrex, Okex
MOFUSDT|2|4|Bittrex, Okex
NMRBTC|3|9|Bittrex, Poloniex, Upbit
NPXSBTC|4|16|Bittrex, Huobipro, Kucoin, Upbit
NXTBTC|4|16|Bittrex, Indodax, Poloniex, Upbit
OCEANBTC|2|4|Bittrex, Kucoin
OCEANUSDT|2|4|Bittrex, Gateio
ORBSBTC|2|4|Bittrex, Upbit
OXTBTC|2|4|Bittrex, Okex
OXTUSDT|2|4|Bittrex, Okex
PARTBTC|2|4|Bittrex, Upbit
PAXBTC|3|9|Bittrex, Okex, Upbit
PAYBTC|5|25|Bittrex, Gateio, Huobipro, Okex, Upbit
PAYETH|3|9|Bittrex, Gateio, Huobipro
PIBTC|2|4|Bittrex, Upbit
PMABTC|3|9|Bittrex, Okex, Upbit
PXLBTC|2|4|Bittrex, Upbit
QNTBTC|2|4|Bittrex, Upbit
QRLBTC|2|4|Bittrex, Upbit
RADSBTC|2|4|Bittrex, Upbit
RDDBTC|2|4|Bittrex, Upbit
RFRBTC|2|4|Bittrex, Upbit
SBDBTC|2|4|Bittrex, Upbit
SCUSD|2|4|Bittrex, Kraken
SIXBTC|2|4|Bittrex, Liquid
SKMBTC|2|4|Bittrex, Huobipro
SKMUSDT|3|9|Bittrex, Gateio, Huobipro
SOLVEBTC|3|9|Bittrex, Kucoin, Upbit
SPCBTC|2|4|Bittrex, Upbit
SPNDBTC|4|16|Bittrex, Kucoin, Okex, Upbit
SRNBTC|3|9|Bittrex, Huobipro, Upbit
SRNETH|2|4|Bittrex, Huobipro
SUTERBTC|2|4|Bittrex, Kucoin
SUTERUSDT|2|4|Bittrex, Kucoin
TNCBTC|2|4|Bittrex, Gateio
TRACBTC|2|4|Bittrex, Kucoin
TRACETH|2|4|Bittrex, Kucoin
TSHPBTC|2|4|Bittrex, Upbit
TTCBTC|2|4|Bittrex, Upbit
TUSDBTC|3|9|Bittrex, Okex, Upbit
UBQBTC|2|4|Bittrex, Upbit
UBTBTC|2|4|Bittrex, Liquid
UKGBTC|2|4|Bittrex, Upbit
UPPBTC|2|4|Bittrex, Upbit
USDCBTC|2|4|Bittrex, Okex
USDTEUR|2|4|Bittrex, Kraken
UTKBTC|3|9|Bittrex, Huobipro, Kucoin
VBKBTC|2|4|Bittrex, Upbit
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
XTZETH|4|16|Bittrex, Gateio, Huobipro, Kraken
XUCUSDT|2|4|Bittrex, Okex
XVGUSDT|2|4|Bittrex, Gateio
YOUBTC|2|4|Bittrex, Okex
BTCBRL|2|4|Coinbase, Ftx
BTCCAD|2|4|Coinbase, Kraken
BTCCHF|2|4|Coinbase, Kraken
BTCHKD|2|4|Coinbase, Liquid
BTCIDR|2|4|Coinbase, Indodax
BTCSGD|3|9|Coinbase, Itbit, Liquid
LINKEUR|2|4|Coinbasepro, Kraken
OMGEUR|2|4|Coinbasepro, Kraken
XTZEUR|2|4|Coinbasepro, Kraken
ETHDAI|6|36|Coinbasepro, Kraken, Kucoin, Liquid, Okex, Poloniex
ALGOEUR|2|4|Coinbasepro, Kraken
ETCEUR|2|4|Coinbasepro, Kraken
BALUSDT|3|9|Ftx, Okex, Poloniex
CUSDTUSDT|2|4|Ftx, Poloniex
DMGUSDT|2|4|Ftx, Okex
MTAUSDT|3|9|Ftx, Gateio, Poloniex
PAXGUSD|2|4|Ftx, Kraken
SOLUSDT|2|4|Ftx, Gateio
YFIUSDT|3|9|Ftx, Gateio, Poloniex
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
BTMUSDT|3|9|Gateio, Huobipro, Okex
SNTUSDT|3|9|Gateio, Huobipro, Okex
PAYUSDT|2|4|Gateio, Okex
PSTUSDT|2|4|Gateio, Okex
BTGUSDT|2|4|Gateio, Okex
AEUSDT|2|4|Gateio, Huobipro
REQETH|3|9|Gateio, Huobipro, Kucoin
MDAUSDT|2|4|Gateio, Okex
GNTUSDT|4|16|Gateio, Huobipro, Okex, Poloniex
ABTUSDT|2|4|Gateio, Okex
ABTETH|3|9|Gateio, Huobipro, Okex
OCNUSDT|2|4|Gateio, Huobipro
OCNETH|2|4|Gateio, Huobipro
OCNBTC|2|4|Gateio, Huobipro
COFIETH|2|4|Gateio, Kucoin
RUFFUSDT|2|4|Gateio, Huobipro
RUFFETH|2|4|Gateio, Huobipro
RUFFBTC|2|4|Gateio, Huobipro
SMTUSDT|2|4|Gateio, Huobipro
SMTETH|2|4|Gateio, Huobipro
MDTETH|2|4|Gateio, Okex
MANAUSDT|4|16|Gateio, Huobipro, Okex, Poloniex
ELFUSDT|3|9|Gateio, Huobipro, Okex
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
BCDUSDT|2|4|Gateio, Okex
SBTCBTC|3|9|Gateio, Huobipro, Okex
BCXBTC|3|9|Gateio, Huobipro, Okex
GNXETH|3|9|Gateio, Huobipro, Okex
GASUSDT|2|4|Gateio, Okex
NASUSDT|3|9|Gateio, Huobipro, Okex
BTMETH|4|16|Gateio, Huobipro, Kucoin, Okex
GTBTC|2|4|Gateio, Huobipro
GTUSDT|2|4|Gateio, Huobipro
RSRUSDT|3|9|Gateio, Huobipro, Liquid
KAIUSDT|2|4|Gateio, Kucoin
KSMUSDT|3|9|Gateio, Huobipro, Kucoin
DOTUSDT|3|9|Gateio, Huobipro, Okex
XEMUSDT|4|16|Gateio, Huobipro, Kucoin, Okex
BUETH|2|4|Gateio, Kucoin
BUBTC|2|4|Gateio, Kucoin
BTC3LUSDT|2|4|Gateio, Liquid
BTC3SUSDT|2|4|Gateio, Liquid
ETH3LUSDT|2|4|Gateio, Liquid
ETH3SUSDT|2|4|Gateio, Liquid
BCNUSDT|2|4|Gateio, Poloniex
STEEMUSDT|3|9|Gateio, Huobipro, Poloniex
ATPUSDT|2|4|Gateio, Huobipro
KLAYUSDT|2|4|Gateio, Liquid
GRINETH|2|4|Gateio, Kucoin
BTTETH|4|16|Gateio, Huobipro, Kucoin, Okex
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
LAMBUSDT|3|9|Gateio, Huobipro, Okex
LAMBETH|2|4|Gateio, Huobipro
WICCETH|2|4|Gateio, Huobipro
VIDYUSDT|2|4|Gateio, Huobipro
FTMETH|2|4|Gateio, Kucoin
MTVUSDT|2|4|Gateio, Kucoin
HCETH|4|16|Gateio, Huobipro, Kucoin, Okex
FTIETH|2|4|Gateio, Huobipro
LBAUSDT|3|9|Gateio, Huobipro, Okex
LBAETH|2|4|Gateio, Huobipro
OPENETH|2|4|Gateio, Kucoin
MITHETH|2|4|Gateio, Okex
HTUSDT|2|4|Gateio, Huobipro
MXCBTC|2|4|Gateio, Huobipro
LETUSDT|2|4|Huobipro, Okex
CHATBTC|2|4|Huobipro, Okex
KCASHUSDT|2|4|Huobipro, Okex
ALGOETH|4|16|Huobipro, Kraken, Kucoin, Okex
ITCBTC|3|9|Huobipro, Kucoin, Okex
KANBTC|2|4|Huobipro, Okex
AACETH|2|4|Huobipro, Okex
CTXCETH|2|4|Huobipro, Okex
YEEUSDT|2|4|Huobipro, Okex
SWFTCBTC|3|9|Huobipro, Okex, Poloniex
EMUSDT|2|4|Huobipro, Okex
GASETH|2|4|Huobipro, Okex
KCASHETH|2|4|Huobipro, Okex
AACBTC|2|4|Huobipro, Okex
ITCETH|2|4|Huobipro, Kucoin
ACTUSDT|2|4|Huobipro, Okex
EGTUSDT|2|4|Huobipro, Okex
SNCBTC|2|4|Huobipro, Okex
UTKETH|2|4|Huobipro, Kucoin
SOCBTC|2|4|Huobipro, Okex
GNXBTC|2|4|Huobipro, Okex
FSNUSDT|2|4|Huobipro, Okex
ACTETH|2|4|Huobipro, Kucoin
MANBTC|2|4|Huobipro, Kucoin
ELAETH|2|4|Huobipro, Kucoin
WXTBTC|3|9|Huobipro, Kucoin, Okex
TRIOBTC|2|4|Huobipro, Okex
KSMBTC|2|4|Huobipro, Kucoin
NCASHBTC|2|4|Huobipro, Upbit
DATXETH|2|4|Huobipro, Kucoin
MTNBTC|2|4|Huobipro, Kucoin
ETNETH|3|9|Huobipro, Kucoin, Liquid
CMTUSDT|2|4|Huobipro, Okex
KCASHBTC|2|4|Huobipro, Okex
TOPCETH|2|4|Huobipro, Okex
SWFTCETH|2|4|Huobipro, Okex
AKROUSDT|2|4|Huobipro, Kucoin
FAIRETH|2|4|Huobipro, Okex
RSRBTC|2|4|Huobipro, Liquid
VSYSUSDT|3|9|Huobipro, Kucoin, Okex
ITCUSDT|3|9|Huobipro, Kucoin, Okex
ETNBTC|3|9|Huobipro, Kucoin, Liquid
DCRETH|2|4|Huobipro, Kucoin
AACUSDT|2|4|Huobipro, Okex
QUNBTC|2|4|Huobipro, Okex
KANETH|2|4|Huobipro, Okex
EGTBTC|3|9|Huobipro, Kucoin, Okex
ACTBTC|3|9|Huobipro, Kucoin, Okex
DATXBTC|2|4|Huobipro, Kucoin
ELABTC|2|4|Huobipro, Kucoin
LETBTC|2|4|Huobipro, Okex
WXTUSDT|3|9|Huobipro, Kucoin, Okex
TRIOETH|2|4|Huobipro, Okex
SOCUSDT|2|4|Huobipro, Okex
ABTBTC|2|4|Huobipro, Okex
ETHSGD|2|4|Itbit, Liquid
BTCDAI|5|25|Kraken, Kucoin, Liquid, Okex, Poloniex
XRPJPY|2|4|Kraken, Liquid
SNXETH|2|4|Kucoin, Okex
EGTETH|2|4|Kucoin, Okex
CRPTETH|2|4|Kucoin, Liquid
MTCBTC|2|4|Kucoin, Liquid
CRPTBTC|2|4|Kucoin, Liquid
USDTUSDC|2|4|Kucoin, Poloniex
AVAUSDT|2|4|Kucoin, Poloniex
BLOCUSDT|2|4|Kucoin, Okex
ROOBEEBTC|2|4|Kucoin, Liquid
ROADUSDT|2|4|Kucoin, Okex
EWTBTC|2|4|Kucoin, Liquid
PLTUSDT|2|4|Kucoin, Poloniex
AERGOBTC|3|9|Kucoin, Okex, Upbit
AVABTC|2|4|Kucoin, Poloniex
PCIBTC|2|4|Liquid, Upbit
XNKBTC|2|4|Liquid, Upbit
GOM2BTC|2|4|Liquid, Upbit
SWFTCUSDT|2|4|Okex, Poloniex
ETCUSDC|2|4|Okex, Poloniex
BSVUSDC|2|4|Okex, Poloniex


This brings a total possible exact matching permutation count of `13,333`.
