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
A table of supported exchanges in executium for version 2. The following table is the status as of 10th June 2020.

Exchange | Active | Symbols Active
------------ | ------------ | ------------
Binance|Yes|583
Bitfinex|Yes|294
Bitflyer|Yes|0
Bithumb|Yes|109
Bitmart|Yes|0
Bitmax|Yes|201
Bitmex|Yes|13
Bitstamp|Yes|15
Bittrex|Yes|415
Coinbase|Yes|0
Coinbasepro|Yes|59
Coincheck|Yes|0
Deribit|Yes|8
Ftx|Yes|288
Gateio|Yes|469
Huobipro|Yes|558
Indodax|Yes|0
Itbit|Yes|0
Kraken|Yes|155
Kucoin|Yes|437
Liquid|Yes|176
Okex|Yes|365
Poloniex|Yes|149
Upbit|Yes|259

## Supported Symbols in Version 2
We have increased our symbols and exchange support with version 2, as of the 10th June 2020 (https://executium.com/symbols-exchanges-marketspreads/). 

Version | Exchanges Supported | Symbols Supported | Market Spreads
------------ | ------------ | ------------  | ------------
Version 2|24|4,553|10,362,628
Version 1|12|140|869

We are adding and updating symbols supported by executium daily, the list for [Symbols Supported](./symbols-supported.md) can be monitored. We intend to update this support list weekly with version 2, and for a real-time look at support you can access via the api endpoint `system/symbols` for a full list of support symbols, or keep up to date in real-time via the executium website.
