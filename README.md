![Executium API Version 2](https://i.imgur.com/IqQoZzi.png)

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
[executium-brand-guidelines.pdf](./executium-brand-guidelines.pdf) | Brand guidelines for executium version 2.

## Supported Exchanges in Version 2
The following table is the status as of 31st July 2021.

Exchange | Executium Code |Active | Symbols Count
------------ | ------------ | ------------ | ------------
Binance|binance|Yes|1177
Binancecoinm|binancecoinm|Yes|36
Binanceusdm|binanceusdm|Yes|122
Bitfinex2|bitfinex version 2|Yes|340
Bitflyer|bitflyer|Yes|13
Bithumb|bithumb|Yes|248
Bitmart|bitmart|Yes|5
Bitmex|bitmex|Yes|34
Bitstamp|bitstamp|Yes|96
Bittrex|bittrex|Yes|948
Bybit|bybit|Yes|28
Coinbase|coinbase|Yes|166
Coinbasepro|coinbasepro|Yes|244
Coincheck|coincheck|Yes|5
Deribit|deribit|Yes|16
Ftx|ftx|Yes|693
Gateio|gateio|Yes|1644
Hitbtc|hitbtc|Yes|1248
Huobipro|huobipro|Yes|908
Indodax|indodax|Yes|150
Kraken|kraken|Yes|364
Krakenfutures|krakenfutures|Yes|17
Kucoin|kucoin|Yes|790
Liquid|liquid|Yes|217
Okex|okex|Yes|478
Okex5|okex version 5|Yes|478
Poloniex|poloniex|Yes|349


## Supported Symbols in Version 2
We have increased our symbols and exchange support with version 2, as of the 31st July 2021

Version | Exchanges | Pairs | Combinations | Permutation 
------------ | ------------ | ------------  | ------------   | ------------
Version 2|31|9,303|43,268,253|86,536,506
Version 1|12|138|871 | 871
### Quote to Quote Permutation

Quote | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
BTC|2447|5,987,809|Binance, Bitflyer, Bithumb, Bitmart, Bittrex, Coinbasepro, Ftx, Hitbtc, Kucoin, Liquid, Okex, Okex5, Poloniex
ETH|1534|2,353,156|Binance, Bittrex, Coinbasepro, Hitbtc, Kucoin, Liquid, Okex, Okex5, Poloniex
USDT|3224|10,394,176|Binance, Binanceusdm, Bitmart, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
BNB|130|16,900|Binance, Poloniex
TUSD|28|784|Binance, Hitbtc, Kucoin, Poloniex
PAX|18|324|Binance, Bitmart, Hitbtc, Kucoin, Poloniex
USDC|94|8,836|Binance, Bitmart, Coinbasepro, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
TRX|35|1,225|Binance, Kucoin, Poloniex
BUSD|211|44,521|Binance, Binanceusdm, Hitbtc, Poloniex
NGN|3|9|Binance, Coinbase
RUB|15|225|Binance, Coinbase
TRY|27|729|Binance, Coinbase
EUR|143|20,449|Binance, Bitflyer, Bitmex, Bittrex, Coinbase, Coinbasepro, Ftx, Liquid
IDRT|5|25|Binance, Hitbtc, Liquid
GBP|66|4,356|Binance, Coinbase, Coinbasepro
UAH|6|36|Binance, Coinbase
BIDR|12|144|Binance
AUD|16|256|Binance, Coinbase, Liquid
DAI|34|1,156|Binance, Coinbasepro, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
BRL|22|484|Binance, Coinbase
BVND|2|4|Binance
VAI|2|4|Binance
USD|1245|1,550,025|Binancecoinm, Bitflyer, Bitmex, Bittrex, Bybit, Coinbase, Coinbasepro, Deribit, Ftx, Hitbtc, Liquid
JPY|20|400|Bitflyer, Coinbase, Liquid
KRW|178|31,684|Bithumb, Coinbase
XBT|7|49|Bitmex
CHF|6|36|Coinbase, Kraken
HKD|3|9|Coinbase, Liquid
IDR|142|20,164|Coinbase
SGD|10|100|Coinbase, Liquid
BRZ|2|4|Ftx
HIT|23|529|Hitbtc
EOS|15|225|Hitbtc
DDRST|4|16|Hitbtc
EURS|11|121|Hitbtc
BCH|25|625|Hitbtc
EOSDT|7|49|Hitbtc
GUSD|4|16|Hitbtc
ZAUD|20|400|Kraken
XETH|44|1,936|Kraken
ZEUR|77|5,929|Kraken
ZGBP|39|1,521|Kraken
ZUSD|82|6,724|Kraken, Liquid
XXBT|67|4,489|Kraken
ZJPY|9|81|Kraken
ZCAD|6|36|Kraken
KCS|27|729|Kucoin
UST|12|144|Kucoin
GYEN|3|9|Liquid
OKB|6|36|Okex, Okex5
USDK|30|900|Okex, Okex5
USDJ|3|9|Poloniex

### Base to Base Permutation

Base | Markets | Permutation | Exchanges
------------ | ------------ | ------------ | ------------
ETH|118|13,924|Binance, Binancecoinm, Binanceusdm, Bitflyer, Bithumb, Bitmart, Bitmex, Bittrex, Bybit, Coinbasepro, Deribit, Ftx, Hitbtc, Kucoin, Liquid, Okex, Okex5, Poloniex
LTC|74|5,476|Binance, Binancecoinm, Binanceusdm, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kucoin, Liquid, Okex, Okex5, Poloniex
BNB|44|1,936|Binance, Binancecoinm, Binanceusdm, Bithumb, Bitmex, Bybit, Ftx, Hitbtc, Kucoin, Poloniex
NEO|39|1,521|Binance, Binanceusdm, Bittrex, Ftx, Hitbtc, Kucoin, Okex, Okex5, Poloniex
QTUM|35|1,225|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
EOS|70|4,900|Binance, Binancecoinm, Binanceusdm, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
SNT|20|400|Binance, Bithumb, Bittrex, Hitbtc, Kucoin, Okex, Okex5, Poloniex
BNT|30|900|Binance, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Okex, Okex5, Poloniex
BTC|287|82,369|Binance, Binancecoinm, Binanceusdm, Bitflyer, Bithumb, Bitmart, Bittrex, Bybit, Coinbase, Coinbasepro, Deribit, Ftx, Hitbtc, Kucoin, Liquid, Okex, Okex5, Poloniex
LRC|27|729|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kucoin, Okex, Okex5, Poloniex
OMG|46|2,116|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
ZRX|45|2,025|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
KNC|39|1,521|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
IOTA|23|529|Binance, Binanceusdm, Bittrex, Ftx, Hitbtc, Okex, Okex5
LINK|72|5,184|Binance, Binancecoinm, Binanceusdm, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
ETC|54|2,916|Binance, Binancecoinm, Binanceusdm, Bithumb, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kucoin, Okex, Okex5, Poloniex
ZEC|37|1,369|Binance, Binanceusdm, Coinbasepro, Ftx, Hitbtc, Kucoin, Okex, Okex5, Poloniex
DASH|42|1,764|Binance, Binanceusdm, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
TRX|62|3,844|Binance, Binancecoinm, Binanceusdm, Bithumb, Bitmex, Bittrex, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
XRP|84|7,056|Binance, Binancecoinm, Binanceusdm, Bitflyer, Bithumb, Bitmex, Bittrex, Bybit, Ftx, Hitbtc, Kucoin, Liquid, Okex, Okex5, Poloniex
ENJ|38|1,444|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5
STORJ|24|576|Binance, Binanceusdm, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Okex, Okex5, Poloniex
XMR|34|1,156|Binance, Binanceusdm, Ftx, Hitbtc, Kucoin, Okex, Okex5, Poloniex
BAT|43|1,849|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
LSK|25|625|Binance, Bittrex, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
MANA|39|1,521|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
ADA|64|4,096|Binance, Binancecoinm, Binanceusdm, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5
XLM|50|2,500|Binance, Binancecoinm, Binanceusdm, Bitflyer, Bithumb, Bitmex, Bittrex, Coinbasepro, Ftx, Hitbtc, Kucoin, Liquid, Okex, Okex5
WAVES|32|1,024|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5
ICX|25|625|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kraken, Okex, Okex5
IOST|27|729|Binance, Binanceusdm, Bithumb, Bittrex, Hitbtc, Kucoin, Okex, Okex5
NANO|24|576|Binance, Hitbtc, Kraken, Kucoin, Okex, Okex5
ZIL|29|841|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kucoin, Okex, Okex5
ONT|31|961|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kucoin, Okex, Okex5
XEM|32|1,024|Binance, Binanceusdm, Bithumb, Bittrex, Bybit, Ftx, Hitbtc, Kucoin, Liquid, Okex, Okex5, Poloniex
ZEN|20|400|Binance, Binanceusdm, Bittrex, Hitbtc, Kucoin, Okex, Okex5
CVC|20|400|Binance, Binanceusdm, Bittrex, Coinbasepro, Hitbtc, Kucoin, Okex, Okex5, Poloniex
THETA|25|625|Binance, Binancecoinm, Binanceusdm, Bithumb, Ftx, Hitbtc, Kucoin, Okex, Okex5
SC|27|729|Binance, Binanceusdm, Bittrex, Ftx, Hitbtc, Kraken, Okex, Okex5, Poloniex
VET|28|784|Binance, Binanceusdm, Bithumb, Bitmex, Bittrex, Ftx, Hitbtc, Kucoin
DCR|20|400|Binance, Bittrex, Hitbtc, Kucoin, Okex, Okex5, Poloniex
BCH|76|5,776|Binance, Binancecoinm, Binanceusdm, Bitflyer, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
REN|35|1,225|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
USDC|27|729|Binance, Bittrex, Coinbasepro, Kraken, Kucoin, Liquid, Okex, Okex5
BTT|37|1,369|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kucoin, Okex, Okex5, Poloniex
MATIC|47|2,209|Binance, Binanceusdm, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
ATOM|47|2,209|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
ALGO|40|1,600|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5
DOGE|58|3,364|Binance, Binancecoinm, Binanceusdm, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kucoin, Liquid, Okex, Okex5, Poloniex
ANKR|24|576|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Hitbtc, Kraken, Kucoin
CHZ|36|1,296|Binance, Binanceusdm, Bithumb, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5
BAND|26|676|Binance, Binanceusdm, Bittrex, Coinbasepro, Ftx, Hitbtc, Okex, Okex5, Poloniex
XTZ|47|2,209|Binance, Binanceusdm, Bithumb, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
HBAR|26|676|Binance, Binanceusdm, Bittrex, Ftx, Hitbtc, Liquid, Okex, Okex5
USDT|41|1,681|Binance, Bittrex, Coinbasepro, Ftx, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
OGN|20|400|Binance, Binanceusdm, Bittrex, Coinbasepro, Hitbtc, Kraken, Kucoin
SOL|39|1,521|Binance, Binanceusdm, Bitmex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Okex, Okex5
CHR|20|400|Binance, Binanceusdm, Bithumb, Ftx, Hitbtc, Kucoin, Poloniex
DGB|23|529|Binance, Binanceusdm, Bittrex, Hitbtc, Kucoin, Okex, Okex5
COMP|40|1,600|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
SXP|26|676|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kucoin, Poloniex
SNX|48|2,304|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
MKR|47|2,209|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
BAL|34|1,156|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Okex, Okex5, Poloniex
YFI|41|1,681|Binance, Binanceusdm, Bithumb, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
SRM|22|484|Binance, Binanceusdm, Bithumb, Ftx, Hitbtc, Kraken, Okex, Okex5, Poloniex
ANT|20|400|Binance, Bittrex, Hitbtc, Kraken, Okex, Okex5
CRV|40|1,600|Binance, Binanceusdm, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
SAND|28|784|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
DOT|61|3,721|Binance, Binancecoinm, Binanceusdm, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
LUNA|25|625|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kucoin, Okex, Okex5
RSR|27|729|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Liquid, Okex, Okex5, Poloniex
WBTC|28|784|Binance, Bittrex, Coinbasepro, Ftx, Hitbtc, Kucoin, Okex, Okex5, Poloniex
SUSHI|38|1,444|Binance, Binanceusdm, Bithumb, Bitmex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
KSM|34|1,156|Binance, Binanceusdm, Bithumb, Bittrex, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5
UMA|26|676|Binance, Bithumb, Bittrex, Coinbasepro, Hitbtc, Kucoin, Okex, Okex5, Poloniex
UNI|50|2,500|Binance, Binancecoinm, Binanceusdm, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
OXT|21|441|Binance, Bithumb, Bittrex, Coinbasepro, Hitbtc, Kraken, Okex, Okex5
AVAX|25|625|Binance, Binanceusdm, Bittrex, Ftx, Kucoin, Okex, Okex5
AAVE|57|3,249|Binance, Binanceusdm, Bithumb, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
NEAR|21|441|Binance, Binanceusdm, Ftx, Hitbtc, Kucoin, Okex, Okex5
FIL|44|1,936|Binance, Binancecoinm, Binanceusdm, Bitmex, Bittrex, Bybit, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
AXS|20|400|Binance, Binanceusdm, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
GRT|44|1,936|Binance, Binanceusdm, Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Kucoin, Okex, Okex5, Poloniex
1INCH|27|729|Binance, Binanceusdm, Bittrex, Coinbasepro, Ftx, Hitbtc, Kucoin, Okex, Okex5
MIR|20|400|Binance, Coinbasepro, Hitbtc, Kucoin, Okex, Okex5, Poloniex
ICP|25|625|Binance, Binanceusdm, Coinbasepro, Ftx, Hitbtc, Kucoin, Okex, Okex5
LPT|21|441|Binance, Bithumb, Coinbasepro, Hitbtc, Kraken, Kucoin, Liquid, Okex, Okex5, Poloniex
NU|21|441|Binance, Bithumb, Coinbasepro, Hitbtc, Okex, Okex5, Poloniex
FLOW|23|529|Binance, Ftx, Hitbtc, Kraken, Okex, Okex5
DAI|23|529|Bithumb, Bittrex, Coinbasepro, Ftx, Hitbtc, Kraken, Okex, Okex5, Poloniex
BSV|25|625|Bithumb, Bittrex, Ftx, Hitbtc, Okex, Okex5
CRO|22|484|Bithumb, Bittrex, Ftx, Kucoin, Okex, Okex5
