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

We are adding and updating symbols supported by executium daily, the list for [Symbols Supported](./symbols-supported.md) can be monitored. We intend to update this support list weekly with version 2, and for a real-time look at support you can access via the api endpoint `system/symbols` for a full list of support symbols, or keep up to date in real-time via the executium website.
