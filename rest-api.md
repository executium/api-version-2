**Table of Contents**

- [Accessibility](#accessibility)
- [General Information](#general-information)
- [HTTP Return Codes](#http-return-codes)
- [Error Codes](#error-codes)
- [General Information on Endpoints](#general-information-on-endpoints)
- System
	- [Check Server Time](#check-server-time) (system/timestamp)
	- [Endpoints](#endpoints) (system/endpoints)
	- [Ping REST API](#ping-rest-api) (system/ping)
	- [Information](#information) (system/information)
	- [List Validation Functions](#list-validation-functions) (system/list-validation-functions)
	- [Symbols](#symbols) (system/symbols)
	- [System Status](#system-status) (system/status)
	- [List Announcements](#list-announcements) (system/list-announcements)
	- [Exchanges](#exchanges) (system/exchanges)
- Subscriptions
	- [Subscriptions Details](#subscriptions-details) (subscriptions/details)
	- [Cancel Subscription](#cancel-subscription) (subscriptions/cancel)
	- [Commissions Report](#commissions-report) (subscriptions/commissions-report)
	- [Deposit Addresses](#deposit-addresses) (subscriptions/deposit)
	- [Invoices](#invoices) (subscriptions/invoices)
	- [Change Subscription Package](#change-subscription-package) (subscriptions/change-php-sdk)
	- [Change Setting](#change-setting) (subscriptions/change-setting-request)
	- [Disable Private Server](#disable-private-server) (subscriptions/disable-private-server)
	- [Subscriptions Disable Shared Server](#subscriptions-disable-shared-server) (subscriptions/disable-shared-server)
	- [Enable Private Server](#enable-private-server) (subscriptions/enable-private-server)
	- [Enable Shared Server](#enable-shared-server) (subscriptions/enable-shared-server)
	- [List Private Servers](#list-private-servers) (subscriptions/list-private-servers)
	- [List Shared Servers](#list-shared-servers) (subscriptions/list-shared-servers)
	- [Package Recommendation](#package-recommendation) (subscriptions/php-sdk-recommendation)
	- [Commissions Rate](#commissions-rate) (subscriptions/commissions-rate)
	- [List Packages](#list-packages) (subscriptions/list-packages)
	- [Change Setting Confirm](#change-setting-confirm) (subscriptions/change-setting-confirm)
	- [Subscriptions Server Types](#subscriptions-server-types) (subscriptions/server-types)
	- [Subscriptions Change Package](#subscriptions-change-package) (subscriptions/change-package)
	- [Subscriptions Package Recommendation](#subscriptions-package-recommendation) (subscriptions/package-recommendation)
- Exchange API Keys
	- [Add Exchange API Credentials](#add-exchange-api-credentials) (exchange-api-keys/add)
	- [Test API Key Status](#test-api-key-status) (exchange-api-keys/test)
	- [Delete Exchange API Key](#delete-exchange-api-key) (exchange-api-keys/delete)
	- [Update Exchange API Key](#update-exchange-api-key) (exchange-api-keys/edit)
	- [List Exchange API Keys](#list-exchange-api-keys) (exchange-api-keys/list)
- Strategy
	- [Create Profile Strategy](#create-profile-strategy) (strategy/create-profile)
	- [Create Profile Strategy](#create-profile-strategy) (strategy/edit-profile)
	- [Delete Profile Strategy](#delete-profile-strategy) (strategy/delete-profile)
	- [Strategy High Level Overview](#strategy-high-level-overview) (strategy/high-level-overview)
	- [User Strategy List](#user-strategy-list) (strategy/data/list)
	- [List All Trading Algorithms](#list-all-trading-algorithms) (strategy/list-algorithms)
	- [Exchange List](#exchange-list) (strategy/list-exchanges)
	- [List Profiles](#list-profiles) (strategy/list-profiles)
	- [Debug Data](#debug-data) (strategy/data/debug)
	- [Save Template](#save-template) (strategy/save-template)
	- [Strategy List Templates](#strategy-list-templates) (strategy/list-templates)
	- [Strategy Start](#strategy-start) (strategy/start)
	- [Strategy Stop](#strategy-stop) (strategy/stop)
	- [List Strategies](#list-strategies) (strategy/list-strategies)
	- [List Strategy Transactions](#list-strategy-transactions) (strategy/list-strategy-transactions)
	- [Stop All Strategies](#stop-all-strategies) (strategy/stop-all-strategies)
	- [Strategy Update](#strategy-update) (strategy/update)
	- [List Strategy Options](#list-strategy-options) (strategy/list-strategy-options)
	- [List Watchlist](#list-watchlist) (strategy/list-watchlist)
	- [Add to Watchlist](#add-to-watchlist) (strategy/add-watchlist-item)
	- [Delete Watchlist Item](#delete-watchlist-item) (strategy/delete-watchlist-item)
- Public
	- [Spreads](#spreads) (public/spreads/data)
	- [Fetch Symbol Price](#fetch-symbol-price) (public/fetch-symbol-price)
	- [Bitcoin Price Tracker](#bitcoin-price-tracker) (public/bitcoin-price-tracker)
	- [Fetch Symbol Trades](#fetch-symbol-trades) (public/fetch-symbol-trades)
	- [Realtime Bitcoin Profit](#realtime-bitcoin-profit) (public/realtime-bitcoin-profit)
	- [Exchange Information](#exchange-information) (public/exchange-information)
	- [Tradingview Charts](#tradingview-charts) (public/tradingview-charts)
	- [Trending News Data](#trending-news-data) (public/trending-news-data)
	- [Trending News Watchlist](#trending-news-watchlist) (public/trending-news-watchlist)
	- [Trending News Sources](#trending-news-sources) (public/trending-news-sources)
	- [Trending News Statistics](#trending-news-statistics) (public/trending-news-statistics)
	- [Trending News Source Impact](#trending-news-source-impact) (public/trending-news-source-impact)
	- [Trending News Add Keyword](#trending-news-add-keyword) (public/trending-news-add-keyword)
	- [List your own keywords](#list-your-own-keywords) (public/trending-news-list-my-keywords)
	- [Trending News Remove Keyword](#trending-news-remove-keyword) (public/trending-news-remove-keyword)
	- [Match Pair](#match-pair) (public/match-pair)
	- [Fetch Spread Data](#fetch-spread-data) (public/fetch-spread-data)
	- [Fetch Articles](#fetch-articles) (public/fetch-articles)
	- [Bitcoin Information](#bitcoin-information) (public/bitcoin-information)
	- [Spreads List](#spreads-list) (public/spreads-list)
	- [Supported Wallets](#supported-wallets) (public/supported-wallets)
- Subaccounts
	- [Create Sub Account](#create-sub-account) (subaccounts/subaccount-create)
	- [Edit Subaccount](#edit-subaccount) (subaccounts/subaccount-edit)
	- [Delete Subaccount](#delete-subaccount) (subaccounts/subaccount-delete)
	- [List All Subaccounts](#list-all-subaccounts) (subaccounts/subaccount-list)
	- [Send Broadcast](#send-broadcast) (subaccounts/broadcast-create)
	- [Delete Broadcast](#delete-broadcast) (subaccounts/broadcast-delete)
	- [Edit Broadcast](#edit-broadcast) (subaccounts/broadcast-edit)
	- [List Broadcast](#list-broadcast) (subaccounts/broadcast-list)
	- [Access History](#access-history) (subaccounts/subaccount-access-history)
- User
	- [Close Account](#close-account) (user/close-account)
	- [User Account Balance](#user-account-balance) (user/account-balance)
	- [User Access History](#user-access-history) (user/access-history)
	- [User Account Details](#user-account-details) (user/account-details)
	- [User List Referrals](#user-list-referrals) (user/list-referrals)
	- [User Active Sessions](#user-active-sessions) (user/active-sessions)
	- [User Security Settings](#user-security-settings) (user/security-settings)
	- [Create Support Ticket](#create-support-ticket) (user/create-support-ticket)
	- [Delete Support Ticket](#delete-support-ticket) (user/delete-support-ticket)
	- [Edit Support Ticket](#edit-support-ticket) (user/edit-support-ticket)
	- [List Support Tickets](#list-support-tickets) (user/list-support-tickets)
- Exchange Query
	- [List of Exchange Queries](#list-of-exchange-queries) (exchange-query/list-exchange-queries)
	- [List of Exchange Requests](#list-of-exchange-requests) (exchange-query/list-exchange-requests)
	- [Delete Exchange Query](#delete-exchange-query) (exchange-query/delete-exchange-query)
	- [Create Query](#create-query) (exchange-query/create-query)
	- [Create Order](#create-order) (exchange-query/order-create)
	- [List Balances](#list-balances) (exchange-query/list-balances)
	- [List Closed Orders](#list-closed-orders) (exchange-query/list-closed-orders)
	- [Exchange Query List Open Orders](#exchange-query-list-open-orders) (exchange-query/list-open-orders)
	- [Exchange Query Order Cancel](#exchange-query-order-cancel) (exchange-query/order-cancel)
	- [Exchange Query Order Check](#exchange-query-order-check) (exchange-query/order-check)
	- [Exchange Query Order Create](#exchange-query-order-create) (exchange-query/order-create)
- Wallets
	- [Wallets Fetch Deposit Address](#wallets-fetch-deposit-address) (wallets/fetch-deposit-address)
	- [Wallets List Balances](#wallets-list-balances) (wallets/list-balances)
	- [Withdraw from wallet](#withdraw-from-wallet) (wallets/withdraw)
- Finance
	- [List Commissions Paid](#list-commissions-paid) (finance/list-commissions-paid)
	- [List Recent Transactions](#list-recent-transactions) (finance/list-recent-transactions)
	- [List Top Strategy PNL](#list-top-strategy-pnl) (finance/list-top-strategy-pnl)
	- [List Deposits](#list-deposits) (finance/list-depoists)
	- [List Withdraws](#list-withdraws) (finance/list-withdraws)
	- [Import Orders List](#import-orders-list) (finance/import-orders-list)
	- [Import Orders Settings](#import-orders-settings) (finance/import-orders-settings)
- Tests
	- [Black Scholes Implied Volatility Calculator](#black-scholes-implied-volatility-calculator) (tests/black-scholes-implied-volatility-calculator)
	- [Test Server Location Speed To Exchange](#test-server-location-speed-to-exchange) (tests/server-location-speed-to-exchange)
- Exchange Index
	- [Exchange Index Announcements](#exchange-index-announcements) (exchangeindex/announcements)
	- [Monitored Exchanges](#monitored-exchanges) (exchangeindex/exchanges)
	- [Relevant News](#relevant-news) (exchangeindex/relevant-news)
	- [Monitored Symbols](#monitored-symbols) (exchangeindex/symbols)
- Export
	- [Export Fetch](#export-fetch) (export/fetch)
	- [Export List](#export-list) (export/list)
	- [Request Export](#request-export) (export/request)
- Calendar
	- [Add Reminder](#add-reminder) (calendar/add-reminder)
	- [List Schedule](#list-schedule) (calendar/list-schedule)
- Algorithm Creator
	- [Algorithm Add](#algorithm-add) (algorithm-creator/algorithm-add)
	- [Algorithm Remove](#algorithm-remove) (algorithm-creator/algorithm-remove)
	- [Algorithm Statistics](#algorithm-statistics) (algorithm-creator/algorithm-statistics)
	- [Algorithm Update](#algorithm-update) (algorithm-creator/algorithm-update)
	- [Condition Add](#condition-add) (algorithm-creator/condition-add)
	- [Condition Remove](#condition-remove) (algorithm-creator/condition-remove)
	- [Condition Update](#condition-update) (algorithm-creator/condition-update)
	- [Execution Add](#execution-add) (algorithm-creator/execution-add)
	- [Execution Remove](#execution-remove) (algorithm-creator/execution-remove)
	- [Execution Update](#execution-update) (algorithm-creator/execution-update)
	- [List Algorithms](#list-algorithms) (algorithm-creator/list-algorithms)
	- [List Condition Operators](#list-condition-operators) (algorithm-creator/list-condition-operators)
	- [List Conditions](#list-conditions) (algorithm-creator/list-conditions)
	- [List Executions](#list-executions) (algorithm-creator/list-executions)
	- [List Order Types](#list-order-types) (algorithm-creator/list-order-types)
	- [Publish Algorithm](#publish-algorithm) (algorithm-creator/publish-algorithm)
	- [Unpublish Algorithm](#unpublish-algorithm) (algorithm-creator/unpublish-algorithm)
	- [Validate Algorithm](#validate-algorithm) (algorithm-creator/validate-algorithm)
- Marketplace
	- [Signal Trigger](#signal-trigger) (marketplace/signals-trigger)
	- [Edit Signal](#edit-signal) (marketplace/signals-edit)
	- [Reset Signal Statistics](#reset-signal-statistics) (marketplace/signal-reset)
	- [Signals Feed](#signals-feed) (marketplace/signals-feed)
	- [Create Signal Profile](#create-signal-profile) (marketplace/signals-add)
	- [Delete Signal](#delete-signal) (marketplace/signal-delete)
	- [Signals Iteration Price Movement](#signals-iteration-price-movement) (marketplace/signals-iteration-price-movement)
- Backtesting
	- [Orderbook Data](#orderbook-data) (backtesting/orderbook-data)
	- [Technical Indicators](#technical-indicators) (backtesting/technical-indicators)
	- [Availability Information](#availability-information) (backtesting/availability)
- Articles
	- [Create Article](#create-article) (articles/create)
	- [List all of your articles](#list-all-of-your-articles) (articles/list)
	- [Delete your article](#delete-your-article) (articles/delete)
	- [Check earnings](#check-earnings) (articles/check-earnings)
	- [Edit your article](#edit-your-article) (articles/edit)


# Public REST API Version 2 for Executium (private beta)

## Accessibility
Currently executium version 2 is in private beta mode as of 10th June 2020. We will update the status of the public release date in this file when decided upon.

## General Information

* Version 2 is currently in private beta.
* The primary base endpoint is: **`[PRIVATE-MODE]`**
* The `trending-news` base is : **`trendingnews.executium.com`**
* The base for public `marketdata` is : **`marketdata.executium.com`**
* All endpoints return either a JSON object or array.
* There are currently **`183 endpoints`** as part of version 2.
* Data returned is limited by default to 10 rows and page 1 in descending order (newest first).
* Timestamp fields vary and are labeled to their corresponding contents of **milliseconds** or **time**

## HTTP Return Codes

* HTTP `4XX` return codes are used for malformed requests where the issue exists with the sender.
* HTTP `422` return code is applied when a user input is unexpected.
* HTTP `429` return code is used when breaking a request rate limit.
* HTTP `418` return code is used when an IP has been banned automatically for continuing to send requests after receiving `429` codes.
* HTTP `5XX` return codes are used for internal errors where the issue is with the executium side.

## Error Codes
* Any endpoint has the ability to return an ERROR

Sample Payload below:
```javascript

"data": {
  "code": 1440,
  "error": "Missing POST parameter(s) required to proceed, review 'missing_parameters' for more information."
},
   
```

* We provide a comprehensive run down on codes in [Errors Codes](./errors.md).

## General Information on Endpoints
* For `POST` endpoints, the parameters must be sent as a `query string` or in the `request body`.
* For `GET` endpoints, parameters must be sent as a `query string`.
* Parameters may be sent in any order.
* If a parameter sent in both the `query string` and `request body`, the `query string` parameter will take priority.

## Check Server Time
Test connectivity to our REST API and get the current server time with a timestamp and millisecond timing.

```
GET /api/v2/system/timestamp
```

**Parameters:**
None

**Successful Response Payload:**
```javascript
{
    "data": {
        "seconds": 1591780920,
        "milliseconds ": 1591780920709
    },
}
```


## Endpoints
A list of all the available endpoints.

```
GET /api/v2/system/endpoints
```

**Parameters:**
None

**Successful Response Payload:**
```javascript
{
    "data": [
        {
            "path": "system/timestamp",
            "parent": "System",
            "name": "Check Server Time",
            "description": "Test connectivity to our REST API and get the current server time with a timestamp and millisecond timing.",
            "auth_required": false,
            "parameters": []
        },
		...
		...
	]
}
```


## Ping REST API
Text the connectivity to the REST API

```
POST /api/v2/system/ping
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
milliseconds |  | NO | 0 | Provide a milliseconds timestamp and then the server will provide a subtracted return value from your input. For more information about millisecond functions visit https://github.com/executium/millisecond-functions


**Successful Response Formatted:**

Name | Example Value
------------ | ------------
our_server_ms | 1591777804071
your_sent_ms | 1591777804158
difference | -87
equation | our_server_ms - your_sent_ms
note | Always make sure your devices time is synchronized for best results.


**Successful Response Payload:**
```javascript
{
  "data": {
    "our_server_ms": 1591777804071,
    "your_sent_ms": "1591777804158",
    "difference": -87,
    "equation": "our_server_ms - your_sent_ms",
    "note": "Always make sure your devices time is synchronized for best results."
  },
  "meta": {
    "api_version": 2,
    "system_version": "2.0.5",
    "status": 200,
    "endpoint": "system/ping",
    "auth_required": false,
    "ms": 1591777804071,
    "time": 1591777804,
    "uid": -1,
    "process_time": "0.000204"
  }
}
```


## Information
Authentication is required as the results will be tailored to your actual subscription criteria. System information concentrates on what is supported in executium from an exchange and symbol perspective.

```
GET /api/v2/system/information
```

**Parameters:**
None

**Successful Response Payload:**
```javascript
"data": {
      "time": 1593065740890,
      "supported": {
        "exchanges": [],
        "symbols": []
      }
    },
```


## List Validation Functions
Every paramter is subjected to a validation method. We provide information on any unsuccessful validation about any validation method which may have failed. For speed of process you can obtain the functions we use for validation. For example, by visiting https://github.com/executium/millisecond-functions you can see the function in `PHP` and `Javascript` which we use for `js_millisecond_update`.

```
GET /api/v2/system/list-validation-functions
```

**Parameters:**
None

**Successful Response Formatted:**

Name | Example Value
------------ | ------------
0 | js_millisecond_update
1 | is_email
2 | password_auth
3 | is_valid_symbol
4 | is_valid_side
5 | is_valid_level


**Successful Response Payload:**
```javascript
{
    "data": [
        "js_millisecond_update",
        "is_email",
        "password_auth",
        "is_valid_symbol",
        "is_valid_side",
        "is_valid_level"
    ]
}
```


## Symbols
All symbols listed and supported on executium. This `endpoint` also accepts `GET`, you can filter the data using the `exchange` parameter, for example `GET /api/v2/system/symbols?exchange=bifinex`.

```
POST /api/v2/system/symbols
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
exchange |  | NO |  | Filter the data by exchange.


**Successful Response Payload:**
```javascript
{
  "data": {
    "binance": [
      {
        "id": "ethbtc",
        "symbol": "ETH/BTC",
        "quote": "BTC",
        "base": "ETH",
        "min": 0.000001,
        "pp": 6,
        "pa": 3
      },
      {
        "id": "ltcbtc",
        "symbol": "LTC/BTC",
        "quote": "BTC",
        "base": "LTC",
        "min": 0.000001,
        "pp": 6,
        "pa": 2
      },
      ...
      ...
      ...
    "bitfinex": [
      {
        "id": "btcusd",
        "symbol": "BTC/USD",
        "quote": "USD",
        "base": "BTC",
        "min": 0.000009999999999999999,
        "pp": 5,
        "pa": -1
      },
      {
        "id": "ltcusd",
        "symbol": "LTC/USD",
        "quote": "USD",
        "base": "LTC",
        "min": 0.000009999999999999999,
        "pp": 5,
        "pa": -1
      },
      ...
      ...

      
```


## System Status
This provides information related to the current setup of the network and how it is performing. Any issues will be first reported here. We recommend checking this endpoint if you have any issues with any component of the system to check if it is a local issue or an issue with executium.

```
GET /api/v2/system/status
```

**Parameters:**
None

**Successful Response Payload:**
```javascript
{
    "data": [
      {
        "name": "Connectivity",
        "status": "running",
        "last_checked": 1593068763898,
        "issues": "None"
      },
      {
        "name": "Strategies",
        "status": "running",
        "last_checked": 1593068686695,
        "issues": "None"
      },
      {
        "name": "Sockets",
        "status": "running",
        "last_checked": 1593068683087,
        "issues": "None"
      },
      {
        "name": "Exchanges",
        "status": "running",
        "last_checked": 1593068687005,
        "issues": "None"
      },
      {
        "name": "Executium.com",
        "status": "running",
        "last_checked": 1593068685179,
        "issues": "None"
      },
      {
        "name": "Executium.pro",
        "status": "running",
        "last_checked": 1593068682645,
        "issues": "None"
      },
      {
        "name": "OrderBooks",
        "status": "running",
        "last_checked": 1593068687762,
        "issues": "None"
      },
      {
        "name": "Trades",
        "status": "running",
        "last_checked": 1593068688303,
        "issues": "None"
      },
      {
        "name": "Support",
        "status": "running",
        "last_checked": 1593068682195,
        "issues": "None"
      }
    ],
}
```


## List Announcements
All company announcements are listed in full detail via this endpoint.

```
POST /api/v2/system/list-announcements
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Exchanges
List of all supported exchanges

```
GET /api/v2/system/exchanges
```

**Parameters:**
None

**Successful Response Payload:**
```javascript

{
   "data":[
      {
         "code":"bitfinex",
         "name":"Bitfinex"
      },
      {
         "code":"binance",
         "name":"Binance"
      },
      ...
      ...    

```


## Subscriptions Details
A breakdown on your current subscription with executium. The subscription details provide a full insight into all components of your subscription plan.

```
GET /api/v2/subscriptions/details
```

**Parameters:**
None

**Successful Response Formatted:**

Name | Example Value
------------ | ------------
subscription | See table 'Subscription'
user_settings | See table 'User Settings'
strategies | See table 'Strategies'
subaccounts | See table 'Subaccounts'
exchange_api_keys | See table 'Exchange Api Keys'


### Subscription

Name | Example Value
------------ | ------------
pro_version | 1
enabled | 1
name | Free Basic
price | 0


### User Settings

Name | Example Value
------------ | ------------
enabled | 1
twofactor | 1
private_hosting | 
private_hive | 
api_access | 1
ratelimit | See table 'User Settings => Ratelimit'


### Strategies

Name | Example Value
------------ | ------------
enabled | 1
commissions | 0.002
orderbook_refresh | 500
liquidity_check_maximum | 100
algos_excluded | See table 'Strategies => Algos Excluded'
maximum | See table 'Strategies => Maximum'
ratelimit | See table 'Strategies => Ratelimit'
spread | See table 'Strategies => Spread'
price_offset | See table 'Strategies => Price Offset'
qty_parent | See table 'Strategies => Qty Parent'
qty_child | See table 'Strategies => Qty Child'
sleep_interval | See table 'Strategies => Sleep Interval'
export | See table 'Strategies => Export'
servers | See table 'Strategies => Servers'


### Subaccounts

Name | Example Value
------------ | ------------
enabled | 1
maximum_accounts | 0
qty_parent | See table 'Subaccounts => Qty Parent'
qty_child | See table 'Subaccounts => Qty Child'
exchanges | See table 'Subaccounts => Exchanges'
see_all_strategies | 
export | 
exchange_api_keys | See table 'Subaccounts => Exchange Api Keys'
api_access | 
force_twofactor | 1


### Exchange Api Keys

Name | Example Value
------------ | ------------
enabled | 1
maximum_stored | 3


### User Settings => Ratelimit

Name | Example Value
------------ | ------------
ms | 1000


### Strategies => Algos Excluded

Name | Example Value
------------ | ------------
0 | maker_taker
1 | market_maker_taker
2 | twap
3 | matrix_price_movement


### Strategies => Maximum

Name | Example Value
------------ | ------------
strategies | 10
templates | 3
concurrent_exchange_api_key | 2
duration | 21600


### Strategies => Ratelimit

Name | Example Value
------------ | ------------
orders_per_second | 1


### Strategies => Spread

Name | Example Value
------------ | ------------
maximum | 30
minimum | -30


### Strategies => Price Offset

Name | Example Value
------------ | ------------
maximum | 10
minimum | -10


### Strategies => Qty Parent

Name | Example Value
------------ | ------------
maximum | 0.01
minimum | 0


### Strategies => Qty Child

Name | Example Value
------------ | ------------
maximum | 0.01
minimum | 0


### Strategies => Sleep Interval

Name | Example Value
------------ | ------------
maximum | 30
minimum | 2


### Strategies => Export

Name | Example Value
------------ | ------------
transactions_rows | 10000
maximum_storage_time | 86400


### Strategies => Servers

Name | Example Value
------------ | ------------
speed_testing | 
shared_resource | 1
private_resource | 
locations | Array


### Subaccounts => Qty Parent

Name | Example Value
------------ | ------------
maximum | 1


### Subaccounts => Qty Child

Name | Example Value
------------ | ------------
minimum | 0.5


### Subaccounts => Exchanges

Name | Example Value
------------ | ------------
0 | binance
1 | bitfinex


### Subaccounts => Exchange Api Keys

Name | Example Value
------------ | ------------
share_master | 
add_own | 


**Successful Response Payload:**
```javascript
{
    "data": {
      "subscription": {
        "pro_version": true,
        "enabled": true,
        "name": "Free Basic",
        "price": 0
      },
      "user_settings": {
        "enabled": true,
        "twofactor": true,
        "private_hosting": false,
        "private_hive": false,
        "api_access": true,
        "ratelimit": {
          "ms": 1000
        }
      },
      "strategies": {
        "enabled": true,
        "commissions": 0.002,
        "orderbook_refresh": 500,
        "liquidity_check_maximum": 100,
        "algos_excluded": [
          "maker_taker",
          "market_maker_taker",
          "twap",
          "matrix_price_movement"
        ],
        "maximum": {
          "strategies": 10,
          "templates": 3,
          "concurrent_exchange_api_key": 2,
          "duration": 21600
        },
        "ratelimit": {
          "orders_per_second": 1
        },
        "spread": {
          "maximum": 30,
          "minimum": -30
        },
        "price_offset": {
          "maximum": 10,
          "minimum": -10
        },
        "qty_parent": {
          "maximum": 0.01,
          "minimum": 0
        },
        "qty_child": {
          "maximum": 0.01,
          "minimum": 0
        },
        "sleep_interval": {
          "maximum": 30,
          "minimum": 2
        },
        "export": {
          "transactions_rows": 10000,
          "maximum_storage_time": 86400
        },
        "servers": {
          "speed_testing": false,
          "shared_resource": true,
          "private_resource": false,
          "locations": {
            "private": {
              "active": [],
              "inactive": []
            },
            "shared": {
              "active": [
                "Singapore"
              ],
              "inactive": [
                "Frankfurt",
                "London",
                "Bangalore",
                "Toronto",
                "Amsterdam"
              ]
            }
          }
        }
      },
      "subaccounts": {
        "enabled": true,
        "maximum_accounts": 0,
        "qty_parent": {
          "maximum": 1
        },
        "qty_child": {
          "minimum": 0.5
        },
        "exchanges": [
          "binance",
          "bitfinex"
        ],
        "see_all_strategies": false,
        "export": false,
        "exchange_api_keys": {
          "share_master": false,
          "add_own": false
        },
        "api_access": false,
        "force_twofactor": true
      },
      "exchange_api_keys": {
        "enabled": true,
        "maximum_stored": 3
      }
    },
    "meta": {
      "id": "",
      "api_version": 2,
      "system_version": "2.0.5",
      "status": 200,
      "auth_success": true,
      "rateLimits": {
        "minute": 60
      },
      "subscription": {
        "id": "0",
        "name": "Free"
      },
      "endpoint": "subscriptions/details",
      "auth_required": true,
      "ms": 1592207324028,
      "time": 1592207324,
      "process_time": "0.014913"
    }
}
```


## Cancel Subscription
Ability to cancel your subscription is restricted to the website only currently. Please visit the website to cancel or change your subscription.

```
GET /api/v2/subscriptions/cancel
```

**Parameters:**
None

## Commissions Report
A full list based on date range of your recent commissions due to executium for services rendered. This commission report does not include those which you are paying to the exchanges.

```
GET /api/v2/subscriptions/commissions-report
```

**Parameters:**
None

## Deposit Addresses
List all of your deposit addresses in your account

```
GET /api/v2/subscriptions/deposit
```

**Parameters:**
None

## Invoices
All of your subscription invoices for your period as an executium user. This includes invoices which have been generated where no fee is due. To exclude these please review the filter options.

```
GET /api/v2/subscriptions/invoices
```

**Parameters:**
None

## Change Subscription Package
Provide the ID of the php-sdk you wish to change your current subscription too. You can find the packages `id` via the `subscription/list-packages` endpoint.

```
POST /api/v2/subscriptions/change-php-sdk
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of php-sdk you wish to change too.


## Change Setting
You can change individual settings of a subscription to have more or less of something. Once you make a change your php-sdk will become `custom`. When you request a change you will be provided with a subscription price adjustment `id`.  Use this provided ID with the endpoint `subscriptions/change-setting-confirm`

```
GET /api/v2/subscriptions/change-setting-request
```

**Parameters:**
None

## Disable Private Server
Use the provided `id` from the endpoint `subscriptions/list-private-servers` and confirm the disabling of the server. If you have active strategies currently running on the server it will fail.

```
POST /api/v2/subscriptions/disable-private-server
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | 


## Subscriptions Disable Shared Server
Use the provided `id` from the endpoint `subscriptions/list-shared-servers` and confirm the disabling of the server. If you have active strategies currently running on the server it will fail.

```
POST /api/v2/subscriptions/disable-shared-server
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | 


## Enable Private Server
To enable a private server provide the `region` you would like to have it exist and the `server_package`. There are additional optional criteras for your server configuration. You can consult `subscriptions/server-types` for a full list of options. Please note that when you enable a server it will incur charges as listed in the `subscriptions/server-types` endpoint,

```
POST /api/v2/subscriptions/enable-private-server
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
region |  | YES |  | 
server_package |  | YES |  | Consult `subscriptions/server-types` for a full list of server packages and provide the ID as this parameter


## Enable Shared Server
To enable a shared server provide the `region` you would like to have it exist and the `server_package`. There are additional optional criteras for your server configuration. You can consult `subscriptions/server-types` for a full list of options. Please note that when you enable a server it will incur charges as listed in the `subscriptions/server-types` endpoint,

```
POST /api/v2/subscriptions/enable-shared-server
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
region |  | YES |  | 


## List Private Servers
List all the private servers your currently have on your php-sdk.

```
POST /api/v2/subscriptions/list-private-servers
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## List Shared Servers
List all shared servers currently available to you. These will also include those as defaulted to you by your subscription php-sdk. When you join any subscription, even the free tier of executium, you are nominated servers for your strategies to run on. These provided servers are inclusive of your subscription cost and subject to change by the hour. They will not change if you have an existing strategy running on them.

```
POST /api/v2/subscriptions/list-shared-servers
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Package Recommendation
Based on an array of inputs we will provide a recommended php-sdk for you.

```
GET /api/v2/subscriptions/php-sdk-recommendation
```

**Parameters:**
None

## Commissions Rate
Outputs the current commissions rate that the user is paying per successful transactions. The rate will vary from account to account dependant on their subscription.

```
GET /api/v2/subscriptions/commissions-rate
```

**Parameters:**
None

## List Packages


```
GET /api/v2/subscriptions/list-packages
```

**Parameters:**
None

## Change Setting Confirm


```
GET /api/v2/subscriptions/change-setting-confirm
```

**Parameters:**
None

## Subscriptions Server Types
A full list of available server types are provided. Each with CPU, Memory and other hardware information for your strategy server requirements. You must select if you are wanting to filter `private` or `shared` servers. All prices are included in the list.

```
POST /api/v2/subscriptions/server-types
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
type |  | YES |  | Private or Shared
duration |  | YES |  | Provided in seconds, no less than 7200 seconds. The duration you enter will determine the price.


## Subscriptions Change Package


```
GET /api/v2/subscriptions/change-package
```

**Parameters:**
None

## Subscriptions Package Recommendation


```
GET /api/v2/subscriptions/package-recommendation
```

**Parameters:**
None

## Add Exchange API Credentials
Provide Exchange API credentials for usage with your executium strategies. Once added they will be confirmed and then be made available to strategies.

```
POST /api/v2/exchange-api-keys/add
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
exchange |  | YES |  | See the supported exchanges via the `strategy/list-exchanges` endpoint
label | 6 | YES |  | The label will appear when selecting your API keys for strategies. 
token | 5 | YES |  | API key/token
secret | 4 | YES |  | API secret
password |  | YES |  | Some exchanges, such as OKEx require a password to be provided.


## Test API Key Status
You must use the returned `id` for the keys you wish to test. From this we will run a test to determine if the keys are valid. If they are tested to be invalid then they will also be disabled for selection system-wide.

```
POST /api/v2/exchange-api-keys/test
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide ID of the API key from `exchange-api-keys/list`


## Delete Exchange API Key
Delete a Exchange API Key from your account. In the event that the key is being used by a running strategy you will not be able to remove the key until that has been stopped.

```
POST /api/v2/exchange-api-keys/delete
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of the key you wish to remove.


## Update Exchange API Key


```
POST /api/v2/exchange-api-keys/edit
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID.
label |  | NO |  | Provide the ID of the key you wish to remove.


## List Exchange API Keys
A full list of accessible Exchange API Keys in your account. This will not show the API keys secrets. If a subaccount user is accessing the API key list they will only see according to their permissions.

```
POST /api/v2/exchange-api-keys/list
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Create Profile Strategy
The 

```
POST /api/v2/strategy/create-profile
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
name | 1 | YES |  | 
description |  | NO |  | 


## Create Profile Strategy
The 

```
POST /api/v2/strategy/edit-profile
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID.
name | 1 | YES |  | 
description |  | NO |  | 


## Delete Profile Strategy
The 

```
POST /api/v2/strategy/delete-profile
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id | 1 | YES |  | Provide strategy `id`


## Strategy High Level Overview
A compiled list of the account specified strategy at a high level overview. Most often used in the event you want to keep a stream of latest data on a particular strategy id This data includes what is currently active, inactive and all totals related.

```
GET /api/v2/strategy/high-level-overview
```

**Parameters:**
None

## User Strategy List
A complete list of user created strategies

```
POST /api/v2/strategy/data/list
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## List All Trading Algorithms
A full list of executium trading algorithms. You will be required to reference your subscription to understand which algorithms are available for usage for you on your current strategy.

```
GET /api/v2/strategy/list-algorithms
```

**Parameters:**
None

**Successful Response Payload:**
```javascript
{
    "data": [
        {
            "id": "25",
            "group_name": "CANDLESTICKS",
            "name": "BULLISH HARAMI "
        },
    ]
```


## Exchange List
A full list of exchanges that excutium support

```
GET /api/v2/strategy/list-exchanges
```

**Parameters:**
None

## List Profiles
A full list of profiles on your account.

```
GET /api/v2/strategy/list-profiles
```

**Parameters:**
None

## Debug Data
This is reserved for accounts based on subscription. It allows you to monitor the progress of your running strategy and monitor the performance of the strategy as it runs.

```
GET /api/v2/strategy/data/debug
```

**Parameters:**
None

## Save Template
You can save strategies which you like as templates to use again in the future.

```
POST /api/v2/strategy/save-template
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
copy_strategy_id |  | YES |  | Provide the strategy ID you would like to save as a template.
label |  | YES |  | Optional field. If left blank or not provided the strategy template will be saved as the strategy name.


## Strategy List Templates
List all of your saved strategy templates.

```
GET /api/v2/strategy/list-templates
```

**Parameters:**
None

## Strategy Start
You must specifically call a strategy start event using this endpoint. If you execute this endpoint while a strategy is running nothing will happen. In the event a strategy is running and you request it to start, nothing will happen.

```
POST /api/v2/strategy/start
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide strategy `id`


## Strategy Stop
This endpoint is to specifically tell the strategy to stop. When it has been executed it will attempt to clean up and cancel any pending orders before it fully stops. This can take an unspecified period of time to complete as the system works to confirm that anything pending is completed. You can consult the `force` parameter for a hard stop.

```
POST /api/v2/strategy/stop
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide trategy `id`
force |  | NO |  | If you select to force the stop it will stop immediately and not check to see if the orders are still active at the exchanges. In the event this parameter is used you must cancel the orders yourself via the exchange(s). In the event you start the strategy after a forced stop, the strategy format will reconvene and check any pending orders.


## List Strategies
A complete list of strategies that are actively running on executium.

```
GET /api/v2/strategy/list-strategies
```

**Parameters:**
None

## List Strategy Transactions
Show all strategy transactions related to the `main_id` and `leg_id`. Additional filters can be added such as the current `status`.

```
POST /api/v2/strategy/list-strategy-transactions
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 
main_id |  | YES |  | 
remove_unfilled |  | NO |  | true of false


**Successful Response Payload:**
```javascript
 "data": {
      "transactions": [
        {
          "id": "2002650",
          "time_created": "1593071056",
          "last_updated": "1593071056467",
          "c_active": "1",
          "c_order": "0",
          "c_lookup_status": "0",
          "c_lookup_count": "0",
          "c_row": "0",
          "c_symbol_code": "binance-btcusdc",
          "c_exchange": "binance",
          "c_symbol": "BTC/USDC",
          "c_symbolid": "btcusdc",
          "c_type": "limit",
          "c_type_orig": "maker",
          "c_side": "sell",
          "c_amount": "0.00200000",
          "c_price": "0.00000000",
          "c_price_entry": "9227.11000000",
          "c_price_offset": "60.00000000",
          "c_payload": "{"info":{"symbol":"BTCUSDC","orderId":196785600,"orderListId":-1,"clientOrderId":"execute2000130","transactTime":1593071056427,"price":"9227.11000000","origQty":"0.00200000","executedQty":"0.00000000","cummulativeQuoteQty":"0.00000000","status":"NEW","timeInForce":"GTC","type":"LIMIT","side":"SELL"},"id":"196785600","clientOrderId":"execute2000130","timestamp":1593071056427,"datetime":"2020-06-25T07:44:16.427Z","lastTradeTimestamp":null,"symbol":"BTC/USDC","type":"limit","side":"sell","price":9227.11,"amount":0.002,"cost":0,"average":null,"filled":0,"remaining":0.002,"status":"open","fee":null,"trades":null}",
          "c_time_requested": "1593071056297",
          "c_time_orderplaced": "170",
          "c_time_completed": "1593071056467",
          "c_time_journey": "170",
          "c_order_id": "196785600",
          "c_order_slice": "0",
          "c_order_success": "0",
          "c_order_failed": "0",
          "c_order_status": "open",
          "c_order_remaining": "0.00200000",
          "c_order_filled": "0.00000000",
          "c_com": "0.00000000",
          "c_child_id": "0",
          "c_cancel": "0",
          "c_cancel_time": "0",
          "c_spread_entry": "-7.04000000",
          "c_trace_order": "0",
          "c_conditions": "["spread_greater_than_input_number"]",
          "custom_id": "2000130",
          "c_max_time": "1593071056307",
        },]
}

```


## Stop All Strategies
You can stop all strategies running by execute this endpoint. If you want them to stop at once, look at the `force` paramter for more information.

```
POST /api/v2/strategy/stop-all-strategies
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
force |  | NO |  | If you select to force the stop it will stop all strategies running immediately and not check to see if the orders are still active at the exchanges.


## Strategy Update
Strategies can only be updated when they are stopped. If the strategy is active the update attempt will not be processed.

```
GET /api/v2/strategy/update
```

**Parameters:**
None

## List Strategy Options
List all variables to a strategy. This is a complete set of options available to the executium strategy system,

```
GET /api/v2/strategy/list-strategy-options
```

**Parameters:**
None

## List Watchlist
List all pairs on your watchlist.

```
GET /api/v2/strategy/list-watchlist
```

**Parameters:**
None

## Add to Watchlist
Add code to watchlist.

```
POST /api/v2/strategy/add-watchlist-item
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
code | 1 | YES |  | Provide a executium code to add to your list.


## Delete Watchlist Item
Delete an item from your watchlist

```
POST /api/v2/strategy/delete-watchlist-item
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of your watchlist item. This `id` can be found by reviewing `strategy/list-watchlist`. The code will not be acceptable input.


## Spreads
Data which is served in a public manner and is obtainable via a public call. Additional restrictions may apply and tighter rate limiting. To upgrade your account for faster access please visit executium.

```
GET /api/v2/public/spreads/data
```

**Parameters:**
None

## Fetch Symbol Price
Public API but restrictions apply based on your subscription level. You must provide the exact `symbol` code which executium provides. You can review symbols in the `system/symbols` endpoint. For this endpoint we accept both `POST` and `GET`. An example of `GET` would be `https://marketdata.executium.com/api/v2/public/fetch-symbol-price?code=binance-btcusdt`. 

```
POST /api/v2/public/fetch-symbol-price
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
code |  | YES |  | The executium code, which can be found at [exchanges-supported.md](./exchanges-supported.md) or by calling the endpoint `system/symbols`. This endpoint can taken multiple inputs and is comma delimited. For example you could input `binance-btcusdt,bitfinex-tnbbtc,bitfinex-btcusd`. To a maximum of 10 inputs.


**Successful Response Payload:**
```javascript


  "data": {
    "binance-btcusdt": {
      "bids": {
        "price": 9411.89,
        "qty": 1.756403,
        "time": 1594277450595
      },
      "asks": {
        "price": 9411.9,
        "qty": 0.755546,
        "time": 1594277450595
      }
    },
    "bitfinex-btcusdt": {
      "bids": {
        "price": 9408.5,
        "qty": 0.1,
        "time": 1594277445745
      },
      "asks": {
        "price": 9411.7,
        "qty": 0.1,
        "time": 1594277447627
      }
    },
    "notes": "Refresh rate 1000-1500ms; To adjust please review your subscription."
  },   

```


## Bitcoin Price Tracker
Data related to the current price of Bitcoin in realtime. This endpoint only provides the data streams. You should use your own graph product to map the data. The base endpoint for this should be `marketdata.executium.com`.

```
POST /api/v2/public/bitcoin-price-tracker
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
interval |  | NO | 1000 | Defaults to `1000` milliseconds. Interval options are available at `900`, `750`, `500`, `400`, `250`, `100`, `50` and `25` milliseconds
symbol_filter |  | NO |  | Partial match against symbol


**Successful Response Payload:**
```javascript

{
   "data":{
      "lastupdated":1594190044395,
      "bids":{
         "bitfinex-btcusdt":[
            9274.6,
            0.08127598,
            1594190038305
         ],
         "bitmax-btcusdt":[
            9311.51,
            1.36604,
            1594052693191
         ],
         "binance-btcusdc":[
            9275.56,
            0.160591,
            1594190021947
         ],
         "bittrex-btcusdt":[
            9313.02700719,
            0.09999997,
            1594052659521
         ],
         "bitmart-btcusdc":[
            9308.95,
            0.021205,
            1594052640361
         ],
         ...
         ...
         ...
	"asks":{
         "bitfinex-btcusdt":[
            9277.6,
            0.97142334,
            1594190044336
         ],
         "bitmax-btcusdt":[
            9311.52,
            0.001,
            1594052693191
         ],
         "binance-btcusdc":[
            9281.29,
            0.800595,
            1594190037982
         ],
         "bittrex-btcusdt":[
            9317.6357,
            0.5753,
            1594052659521
         ],
         "bitmart-btcusdc":[
            9319.61,
            0.020239,
            1594052714913
         ],         
   
```


## Fetch Symbol Trades
Fetch the latest trades for a `symbol`. The default is both sides but this can be filtered to `asks` or `bids`

```
POST /api/v2/public/fetch-symbol-trades
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
symbol |  | NO |  | The executium code, which can be found at [exchanges-supported.md](./exchanges-supported.md) or by calling the endpoint `system/symbols`.
side |  | NO | both | Defaults to both sides. Choices: 'both', 'asks' or 'bids'; No other inputs will be accepted.


## Realtime Bitcoin Profit
Showing all of the arbitrage opportunities that show a return - You can use this executium tool to look at the best profit availability on all spreads we monitor. 


```
POST /api/v2/public/realtime-bitcoin-profit
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Exchange Information
Current running and grade information for exchanges that executium supports. The grading is based on a range of factors which can be reviewed here [exchange-grading.md](./exchanges-supported.md)

```
GET /api/v2/public/exchange-information
```

**Parameters:**
None

**Successful Response Payload:**
```javascript
{
    "data": [
      {
        "exchange": "Bitfinex",
        "status": "running",
        "rating": "A"
      },
      {
        "exchange": "Binance",
        "status": "running",
        "rating": "A"
      },
      {
        "exchange": "OKEx",
        "status": "running",
        "rating": "B"
      },
      {
        "exchange": "Binance Futures",
        "status": "running",
        "rating": "C"
      },
      {
        "exchange": "Bitmex",
        "status": "running",
        "rating": "D"
      }
    ],
}
```


## Tradingview Charts
Retrieve the Javascript code for the tradingview chart input. The returned value is the javascript include which can then be included in a page to embed a tradingview chart.

```
POST /api/v2/public/tradingview-charts
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
symbol |  | YES |  | The executium code, which can be found at [exchanges-supported.md](./exchanges-supported.md) or by calling the endpoint `system/symbols`.


## Trending News Data
Trending news data is display on a day per day basis. The date format must be YYYY-MM-DD. You have the additional option to utilize `keyword_contains` which will enable you to pull back all data on keywords which contain your string. This ability is also extended with `title_contains` and `brief_contains`. For multiple keywords to search add a coma (,) onto the string and the system will search for multiple, up to a maximum of 10 per contains.

```
POST /api/v2/public/trending-news-data
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
date | 9 | YES |  | Format YYYY-MM-DD
keyword_contains |  | NO |  | Search for a particular keyword in the `keyword`
title_contains |  | NO |  | Search for a particular keyword in the `title`
brief_contains |  | NO |  | Search for a particular keyword in the `brief`
exclude_keywords |  | NO |  | Coma seperated list of keywords to exclude


**Successful Response Payload:**
```javascript



    "data": [
        {
            "id": "292442",
            "date": {
                "time_published": "1593561844",
                "day": "Wednesday",
                "format1": "2020-07-01",
                "format2": "1st July 2020 00:04"
            },
            "title": "Oil Jumps After API Reports Largest Crude Draw This Year",
            "brief": "Oil prices jumped on Tuesday afternoon after the API reported a large draw in crude oil stocks.",
            "keywords": "oil,crude oil",
            "url": "https://oilprice.com/Latest-Energy-News/World-News/Oil-Jumps-After-API-Reports-Largest-Crude-Draw-This-Year.html",
            "source": "OilPrice.com",
            "image": "",
            "domain": "oilprice.com",
            "author": "Julianne Geiger",
            "price_impact_120s": {
                "status": "Subscription required.",
                "data": []
            },
            "price_impact_300s": {
                "status": "Subscription required.",
                "data": []
            },
            "price_impact_600s": {
                "status": "Subscription required.",
                "data": []
            },
            "price_impact_900s": {
                "status": "Subscription required.",
                "data": []
            },
            "price_impact_1200s": {
                "status": "Subscription required.",
                "data": []
            },
            "price_impact_1800s": {
                "status": "Subscription required.",
                "data": []
            },
            "price_impact_3600s": {
                "status": "completed",
                "data": {
                    "btcusdt": {
                        "status": "compiled",
                        "pair": "BTCUSDT",
                        "before": "9137.30000000",
                        "after": "9126.57000000",
                        "difference": "-10.73000000"
                    },
                    "ethusdt": {
                        "status": "compiled",
                        "pair": "ETHUSDT",
                        "before": "225.59000000",
                        "after": "225.11000000",
                        "difference": "-0.48000000"
                    },
                    "adausdt": {
                        "status": "compiled",
                        "pair": "ADAUSDT",
                        "before": "0.08300000",
                        "after": "0.08295000",
                        "difference": "-0.00005000"
                    },
                    "xrpusdt": {
                        "status": "compiled",
                        "pair": "XRPUSDT",
                        "before": "0.17533000",
                        "after": "0.17484000",
                        "difference": "-0.00049000"
                    },
                    "ethbtc": {
                        "status": "compiled",
                        "pair": "ETHBTC",
                        "before": "0.02468900",
                        "after": "0.02466400",
                        "difference": "-0.00002500"
                    },
                    "adabtc": {
                        "status": "compiled",
                        "pair": "ADABTC",
                        "before": "0.00000909",
                        "after": "0.00000909",
                        "difference": "0.00000000"
                    },
                    "xrpbtc": {
                        "status": "compiled",
                        "pair": "XRPBTC",
                        "before": "0.00001918",
                        "after": "0.00001916",
                        "difference": "-0.00000002"
                    }
                }
            },
            "tone": {
                "status": "Subscription required.",
                "data": []
            }
        },
    ]
      	
	
```


## Trending News Watchlist
This endpoint provides you will the full list of keywords which our trending news topic tracker looks against. 

```
POST /api/v2/public/trending-news-watchlist
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
keyword_contains |  | NO |  | Search for a particular keyword in the keyword


**Successful Response Payload:**
```javascript
 {
    "data": [
      {
        "id": "1",
        "keywords": "btc/usdt",
      },
      {
        "id": "2",
        "keywords": "btcusdt",
      },
      {
        "id": "3",
        "keywords": "bitcoin",
      },
      {
        "id": "4",
        "keywords": "true coin",
      },
      {
        "id": "5",
        "keywords": "ETH/BTC",
      },
}
]
```


## Trending News Sources
A list of all the news sources which have featured in the trending news catalog. Review `public/trending-news-statistics` for more statistics and whole number counts.

```
GET /api/v2/public/trending-news-sources
```

**Parameters:**
None

**Successful Response Payload:**
```javascript
 {
    "data": [
      "3rd Watch News",
      "9to5Mac",
      "About Manchester",
      "Actu Crypto.info",
      "AiThority",
      "allnews.ch",
      "alloaadvertiser.com",
      "Altcoin Buzz",
      "AMBCrypto",
      "AMBCrypto English",
      "AMEinfo",
}
```


## Trending News Statistics
Statistics relating to the trending news catalog. The parameter `total_keywords_matched` can be much higher than total_articles_found as 100s of keywords can be matched to a single article.

```
GET /api/v2/public/trending-news-statistics
```

**Parameters:**
None

**Successful Response Payload:**
```javascript

"data": 
{
	"keywords_monitored": 5235,
	"total_articles_found": 13100,
	"total_keywords_matched": 11372,
	"history": 
	[
		{
		  "added_in_last_hour": 570
		},
		{
		  "last_24_hours": 454
		},
		{
		  "last_48_hours": 725
		},
		{
		  "last_7_days": 2265
		},
		{
		  "last_30_days": 4927
		}
	],
	"sources": 1406,
	"last_update": 1593408099
}	
	
```


## Trending News Source Impact
A complete compiled list to provide insight into news sources impact on prices. You can filter the `source` by using `source_contains`, which will allow you to concentrate on specific sources you want. The `top_ranking_*` array contains the all time list of articles that we have stored and their individual impact.  The `most_recent_*` array provides the most reason `bull` and `bear` articles from the publication.
	
It is important to note, that while some publications seem to have a big impact on price, we are not indicating that they we`re the sole reason for the movement. The intention of this endpoint is to provide additional context to whether the press directly impacts prices or if it is just a fluke.


```
POST /api/v2/public/trending-news-source-impact
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
source_contains | 1 | YES |  | Provide the exact publication you are looking for, for example, if you was looking for the coin telegraph, you would enter the coin telegraph. Consult the source list for more information.


**Successful Response Payload:**
```javascript


"data":
{
	"btcusdt":
	{
		"Cryptonaute":
		{
            "total_articles":410,
            "sum_impact":"590.12000000",
            "top_ranking_bull":[
               {
                  "id":"3836",
                  "keywords":"bitcoin,Ethereum,eth",
                  "time_published":"1587020400",
                  "diff_btcusdt":"233.50000000",
                  "ago":"11 weeks ago"
               },
               {
                  "id":"4011",
                  "keywords":"bitcoin",
                  "time_published":"1592204400",
                  "diff_btcusdt":"90.70000000",
                  "ago":"2 weeks ago"
               },
               {
                  "id":"3831",
                  "keywords":"Ethereum,eth",
                  "time_published":"1589439600",
                  "diff_btcusdt":"63.54000000",
                  "ago":"7 weeks ago"
               },
               {
                  "id":"3777",
                  "keywords":"Ethereum,eth",
                  "time_published":"1592377200",
                  "diff_btcusdt":"37.10000000",
                  "ago":"2 weeks ago"
               },
               {
                  "id":"3839",
                  "keywords":"Ethereum,eth",
                  "time_published":"1589204706",
                  "diff_btcusdt":"34.54000000",
                  "ago":"7 weeks ago"
               }
            ],
            "top_ranking_bear":[
               {
                  "id":"3810",
                  "keywords":"Ethereum,eth",
                  "time_published":"1589918155",
                  "impact":"-16.50000000",
                  "ago":"6 weeks ago"
               }
            ],
            "most_recent_bull":[
               {
                  "id":"4001",
                  "keywords":"bitcoin",
                  "time_published":"1593172260",
                  "diff_btcusdt":"26.14000000",
                  "ago":"3 days ago"
               },
               {
                  "id":"3768",
                  "keywords":"bitcoin,Ethereum,eth",
                  "time_published":"1592910300",
                  "diff_btcusdt":"31.23000000",
                  "ago":"6 days ago"
               },
               {
                  "id":"3773",
                  "keywords":"Ethereum,eth",
                  "time_published":"1592812980",
                  "diff_btcusdt":"10.43000000",
                  "ago":"1 weeks ago"
               },
               {
                  "id":"3792",
                  "keywords":"Ethereum,eth",
                  "time_published":"1592496660",
                  "diff_btcusdt":"2.76000000",
                  "ago":"2 weeks ago"
               },
               {
                  "id":"3777",
                  "keywords":"Ethereum,eth",
                  "time_published":"1592377200",
                  "diff_btcusdt":"37.10000000",
                  "ago":"2 weeks ago"
               }
            ],
            "most_recent_bear":[
               {
                  "id":"3810",
                  "keywords":"Ethereum,eth",
                  "time_published":"1589918155",
                  "impact":"-16.50000000",
                  "ago":"6 weeks ago"
               }
            ]
         },
     },
 }
         	
	
```


## Trending News Add Keyword


```
POST /api/v2/public/trending-news-add-keyword
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
name | 1 | YES |  | The `keyword` you want to track.


**Successful Response Payload:**
```javascript
"data": {
      "code": 2001,
      "error": "Missing Key"
    },
```


## List your own keywords


```
POST /api/v2/public/trending-news-list-my-keywords
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


**Successful Response Payload:**
```javascript
"data": {
      "code": 2001,
      "error": "Missing Key"
    },
```


## Trending News Remove Keyword


```
POST /api/v2/public/trending-news-remove-keyword
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
keywordid |  | YES |  | The `keyword_id` you wish to remove. You can get this information from the `public/trending-news-list-my-keywords` endpoint.


**Successful Response Payload:**
```javascript
"data": {
      "code": 2001,
      "error": "Missing Key"
    },
```


## Match Pair
This system is provided to give insight into a `pairing` and where you can also trade it. For this endpoint we accept both `POST` and `GET`. An example of `GET` would be `https://marketdata.executium.com/api/v2/public/match-pair?code=btcusdt,btcusd`. Please consult the [exchanges-supported.md](./exchanges-supported.md) to understand the scope of where we match.

```
POST /api/v2/public/match-pair
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
code | 1 | YES |  | Provide a pair such as `btcusdt` to discover where else you can trade the pairing `btcusdt`. Comma delimited list acceptable upto 10. Exclude the exchange code from your query and request just the pair like shown.
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


**Successful Response Payload:**
```javascript


{
  "data": {
  
      "BTCUSDT": {
      "pair": "btcusdt",
      "count": 14,
      "active": [
        "Binance",
        "Bitfinex",
        "Bitmart",
        "Bitmax",
        "Bittrex",
        "Ftx",
        "Gateio",
        "Huobipro",
        "Kraken",
        "Kucoin",
        "Liquid",
        "Okex",
        "Poloniex",
        "Upbit"
      ],
      "detail": {
        "binance": {
          "id": "btcusdt",
          "symbol": "BTC/USDT",
          "quote": "USDT",
          "base": "BTC",
          "min": 0.01,
          "pp": 2,
          "pa": 6
        },
        "bitfinex": {
          "id": "btcusdt",
          "symbol": "BTC/USDT",
          "quote": "UST",
          "base": "BTC",
          "min": 0.000009999999999999999,
          "pp": 5,
          "pa": -1
        },
        ...
        ...
        ...

      },
      "possible_combinations": 196
    },
    "BTCUSD": {
      "pair": "btcusd",
      "count": 11,
      "active": [
        "Bitfinex",
        "Bitflyer",
        "Bitmex",
        "Bitstamp",
        "Bittrex",
        "Coinbase",
        "Coinbasepro",
        "Ftx",
        "Itbit",
        "Kraken",
        "Liquid"
      ],
      "detail": {
        "bitfinex": {
          "id": "btcusd",
          "symbol": "BTC/USD",
          "quote": "USD",
          "base": "BTC",
          "min": 0.000009999999999999999,
          "pp": 5,
          "pa": -1
        },
        ...
        ...
        ...
		}
	}
	

```


## Fetch Spread Data
Spreads are calculated as Ask-Bid for price, and Ask/Bid for ratio.

```
POST /api/v2/public/fetch-spread-data
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
combination | 1 | YES |  | Provide a valid combination such as `binance-btcusdt+bitmax-btcusdc`. The `+` acts as a join for the combination. The order is ascending by time.
latestonly |  | NO |  | Set as `true` to activate. Useful to pull when you are only looking to update the latest point
date |  | NO |  | Date of the data. Example 2018-10-12


**Successful Response Payload:**
```javascript


   "data":[
      {
         "price":{
            "open":9.14,
            "close":9.52,
            "high":9.52,
            "low":8.23,
            "time":"1594294380000"
         },
         "ratio":{
            "open":1.001,
            "close":1.001,
            "high":1.001,
            "low":1.0009,
            "time":"1594294380000"
         }
      }
   ],
	
```


## Fetch Articles
Fetch a list of articles published by executium.com

```
POST /api/v2/public/fetch-articles
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
article_id |  | NO | 0 | If `article_id` empty then it will return a list of articles
title_contains |  | NO | 0 | When listing articles it will only return titles that contain the value of `title_contains`
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Bitcoin Information
This endpoint includes data for the market price, market cap, total bitcoins in circulation, difficulty chart, hash rate, miners revenue, cost per transaction, transaction fees and bitcoin trade volumes. This is provided as an information resource.

```
GET /api/v2/public/bitcoin-information
```

**Parameters:**
None

## Spreads List
All spread lists available which are tracked every second of the day. This list works most effectively if you apply a `spread_includes` keyword.

```
POST /api/v2/public/spreads-list
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
spread_includes |  | NO |  | Search for a particular keyword in the spread combination.
limit |  | NO | 100 | 
pagenumber |  | NO | 1 | 


**Successful Response Payload:**
```javascript
"data": {
    "combinations": [
      "binance-btcusdc+bitfinex-btcusdt",
      "binance-btcusdt+bitfinex-btcusdt",
      "bitfinex-btcusdt+binance-btcusdc",
      "bitfinex-btcusdt+binance-btcusdt",
      "bitfinex-btcusdt+bitmart-btcusdc",
      "bitfinex-btcusdt+bitmart-btcusdt",
      "bitfinex-btcusdt+bittrex-btcusdt",
      "bitfinex-btcusdt+coinbasepro-btcusdc",
      "bitfinex-btcusdt+ftx-btcusdt",
      "bitfinex-btcusdt+gateio-btcusdc",
      "bitfinex-btcusdt+gateio-btcusdt",
      "bitfinex-btcusdt+huobipro-btcusdt",
      "bitmart-btcusdc+bitfinex-btcusdt",
      "bitmart-btcusdt+bitfinex-btcusdt",
      "bittrex-btcusdt+bitfinex-btcusdt",
      "coinbasepro-btcusdc+bitfinex-btcusdt",
      "ftx-btcusdt+bitfinex-btcusdt",
      "gateio-btcusdc+bitfinex-btcusdt",
      "gateio-btcusdt+bitfinex-btcusdt",
      "huobipro-btcusdt+bitfinex-btcusdt"
    ],
    "page": 1,
    "showing": 20,
    "total": 20
  },
```


## Supported Wallets
A list of all supported wallets available within executium. These wallets can take deposits which are then used to pay your subscription and commissions due to executium. The list is subject to change.

```
GET /api/v2/public/supported-wallets
```

**Parameters:**
None

**Successful Response Payload:**
```javascript

   "data":{
      "last_updated":1597196783,
      "supported":[
         {
            "symbol":"ADX",
            "name":"AdEx",
            "decimals":4
         },
         {
            "symbol":"AE",
            "name":"Aeternity",
            "decimals":18
         },
         {
            "symbol":"AION",
            "name":"AION",
            "decimals":8
         },
         ...
         ...
         ...
     }
 
         
```


## Create Sub Account
The primary account holder can manage inline with their subscription how many subaccounts can access/create/interact with strategies on their account.

```
POST /api/v2/subaccounts/subaccount-create
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
name | 5 | YES |  | Provide the subaccount users name.
email | 5 | YES |  | Provide the subaccount users e-mail address.
active |  | YES |  | 
parent_maximum |  | YES | 0.1 | Maximum parent in BTC that the subaccount can place per strategy
child_maximum |  | YES | 0.01 | Maximum child in BTC that the subaccount can place per strategy
concurrent_strategies_maximum |  | YES |  | The amount of strategies that the subaccount can run concurrently.
export_enabled |  | YES |  | The subaccount ability to export data (true/true)
view_all_profiles |  | YES |  | Allow user to view all exchange keys
add_exchange_keys |  | YES |  | Ability to add Exchange API Keys to the account.
allow_api_access |  | YES |  | Allow or deny the subaccount access to the account API, in the event the account is given access new API keys for the subaccount will need to be generated (true/true).


## Edit Subaccount
You can edit all basic features about a subaccount but not the `password` or `active status` through the API. To change a subaccount password you must login to the website. If you wish to disable an account use the `subaccounts/subaccount-delete` endpoint,

```
POST /api/v2/subaccounts/subaccount-edit
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of the subaccount.
email | 5 | YES |  | Provide the subaccount users e-mail address.
name | 5 | YES |  | Provide the subaccount users name.
active | 1 | YES |  | 


## Delete Subaccount
You can delete any subaccount by providing the ID, which can be obtain by `list-subaccount`. When you delete a subaccount it will not remove any other related information such as `strategy` or `history`. All information will still eist with the primary account holder.

```
POST /api/v2/subaccounts/subaccount-delete
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of the subaccount.


## List All Subaccounts
Available in subscrition packages. View ID and subaccount information.

```
GET /api/v2/subaccounts/subaccount-list
```

**Parameters:**
None

## Send Broadcast
Send a broadcast to all subaccounts.

```
POST /api/v2/subaccounts/broadcast-create
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
title | 5 | YES |  | The title of the broadcast
body | 5 | YES |  | Provide the body of text to broadcast


## Delete Broadcast
Delete a broadcast you want to remove. Use the `subaccounts/broadcast-list` to locate the `id`.

```
POST /api/v2/subaccounts/broadcast-delete
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of the key you wish to remove.


## Edit Broadcast


```
GET /api/v2/subaccounts/broadcast-edit
```

**Parameters:**
None

## List Broadcast
List all broadcasts

```
POST /api/v2/subaccounts/broadcast-list
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Access History


```
GET /api/v2/subaccounts/subaccount-access-history
```

**Parameters:**
None

## Close Account
If you wish to close your account with executium this is the endpoint. We may require that you close your account via the website.

```
POST /api/v2/user/close-account
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
reason | 10 | YES |  | Please provide feedback and the reasoning for closing your account.
password | 5 | YES |  | Provide your account password.


**Successful Response Formatted:**

Name | Example Value
------------ | ------------
code | 2750
error | Please use the website to close your account.


**Successful Response Payload:**
```javascript
{
    "data": {
        "code": 2750,
        "error": "Please use the website to close your account."
    },
    "meta": {
        "api_version": 2,
        "system_version": "2.0.5",
        "status": 403,
        "auth_success": true,
        "rateLimits": {
            "minute": 60
        },
        "subscription": {
            "id": "0",
            "name": "Free"
        },
        "endpoint": "user/close-account",
        "auth_required": true,
        "ms": 1591779884553,
        "time": 1591779884,
        "uid": 1,
        "process_time": "0.009136"
    }
}
```


## User Account Balance
Show all account balances you have available with executium. This is just for executium wallets which are used to pay your subscriptions and commissions with. If you are looking to check exchanges balances please consult the endpoint `exchange-query/list-balances`

```
GET /api/v2/user/account-balance
```

**Parameters:**
None

## User Access History
A full list of your main accont access activity to the main webite.

```
POST /api/v2/user/access-history
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## User Account Details
Your account information related to properties such as `email` and `name`.

```
GET /api/v2/user/account-details
```

**Parameters:**
None

## User List Referrals
A full list of your recent referrals to the website and the `status` of those referrals and earnings.

```
POST /api/v2/user/list-referrals
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## User Active Sessions
Show all of your current active sessions which are logged into the web system.

```
POST /api/v2/user/active-sessions
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
request | 1 | YES |  | 


## User Security Settings
List all of your security settings and current configuration. These settings apply to your subaccounts also.

```
GET /api/v2/user/security-settings
```

**Parameters:**
None

## Create Support Ticket


```
POST /api/v2/user/create-support-ticket
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
name | 5 | YES |  | 
email | 5 | YES |  | Provide a valid e-mail address
subject | 5 | YES |  | 
category |  | NO |  | 
message | 20 | YES |  | Message must contain at least 20 characters


## Delete Support Ticket


```
POST /api/v2/user/delete-support-ticket
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the support ID


## Edit Support Ticket


```
POST /api/v2/user/edit-support-ticket
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the support ID
name | 5 | YES |  | 
email | 5 | YES |  | Provide a valid e-mail address
subject | 5 | YES |  | 
category |  | NO |  | 
message | 20 | YES |  | Message must contain at least 20 characters


## List Support Tickets


```
POST /api/v2/user/list-support-tickets
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## List of Exchange Queries
This endpoint lists all direct exchanges queries such as balances in a list.

```
GET /api/v2/exchange-query/list-exchange-queries
```

**Parameters:**
None

## List of Exchange Requests


```
GET /api/v2/exchange-query/list-exchange-requests
```

**Parameters:**
None

## Delete Exchange Query
Delete any historical exchange query made. Delete based on `id. This list can be obtained from `exchange-query/list-exchange-queries`

```
POST /api/v2/exchange-query/delete-exchange-query
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | 


## Create Query
Make a request from the exchange

```
POST /api/v2/exchange-query/create-query
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
apikey | 2 | YES |  | Provide API Key ID
exchange_query | 4 | YES |  | Predefined type


## Create Order
Make a request from the exchange

```
POST /api/v2/exchange-query/order-create
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
apikey | 2 | YES |  | Provide API Key ID
ordertype | 4 | YES |  | `market` or `limit`
code | 4 | YES |  | Specify a `executium-code`, for example `bitfinex-btcusdt`
side | 3 | YES |  | `buy` or `sell`
quantity | 1 | YES |  | Specify an order quantity
price |  | NO |  | Related to `ordertype` `limit`.
order_send_time |  | NO |  | The time the first order will be sent. If not provided it will send immediately. Timestamp must be in milliseconds.
repeat_times | 1 | YES | 1 | Defaults to 1. Amount of orders of same settings. The `repeat_interval` will be oberserved. Maximum 10.
repeat_interval | 1 | YES | 10000 | Defaults to 10,000 milliseconds. The time between each order request.
expire_after |  | NO | 0 | Set an expiry time for a `limit` ordertype. Set the milliseconds after the order has been entered in which you wish to cancel.


## List Balances


```
GET /api/v2/exchange-query/list-balances
```

**Parameters:**
None

## List Closed Orders


```
GET /api/v2/exchange-query/list-closed-orders
```

**Parameters:**
None

## Exchange Query List Open Orders


```
GET /api/v2/exchange-query/list-open-orders
```

**Parameters:**
None

## Exchange Query Order Cancel


```
GET /api/v2/exchange-query/order-cancel
```

**Parameters:**
None

## Exchange Query Order Check


```
GET /api/v2/exchange-query/order-check
```

**Parameters:**
None

## Exchange Query Order Create


```
GET /api/v2/exchange-query/order-create
```

**Parameters:**
None

## Wallets Fetch Deposit Address
Select the wallet `type`  you would like to depsoit too. By default it is set to Bitcoin (`BTC`).

```
POST /api/v2/wallets/fetch-deposit-address
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
wallet_currency |  | YES | BTC | 


## Wallets List Balances
List all wallets related to your account for direct purpose of depositing subscription and commission fees too.

```
POST /api/v2/wallets/list-balances
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Withdraw from wallet
Request to withdraw from your executium wallet. You will need to provide the ID and address of the wallet you wish to withdraw from. Please note that only certain subscription levels may have access to this function. Fees apply to process transactions and they can take up to 24 hours as each withdraw request is manually reviewed.

```
POST /api/v2/wallets/withdraw
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
wallet_id |  | YES |  | Find the wallet `id` from the list wallet endpoint
wallet_address |  | YES |  | Find the wallet `address` from the list wallet endpoint
address_to |  | YES |  | Provide the wallet address you wish to transfer too
amount |  | YES |  | Specify the amount to transfer


## List Commissions Paid
This is inclusive of your subaccounts in your account if you have them. All commissions relate directly to executium and not the exchanges commissions taken.

```
POST /api/v2/finance/list-commissions-paid
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
subaccount_id |  | YES |  | Provide a valid subaccount ID from the endpoint `subaccounts/subaccount-list`
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## List Recent Transactions
List all of your most recent transactions related to your executium. This includes your subscription and commissions costs.

```
POST /api/v2/finance/list-recent-transactions
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## List Top Strategy PNL
List all of your most recent strategies and their related profit and loss .

```
POST /api/v2/finance/list-top-strategy-pnl
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## List Deposits
List deposits which have come into executium. This is the deposits which have been made to pay for subscription and commission fees.

```
POST /api/v2/finance/list-depoists
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## List Withdraws
See `wallets/withdraw`

```
GET /api/v2/finance/list-withdraws
```

**Parameters:**
None

## Import Orders List


```
GET /api/v2/finance/import-orders-list
```

**Parameters:**
None

## Import Orders Settings


```
GET /api/v2/finance/import-orders-settings
```

**Parameters:**
None

## Black Scholes Implied Volatility Calculator
Black Scholes Implied Volatility Calculator

```
GET /api/v2/tests/black-scholes-implied-volatility-calculator
```

**Parameters:**
None

## Test Server Location Speed To Exchange
As part of a sound strategy configuration, selecting the right location to run the strategy is essential. The speed test allows you to select an executium server location to ping an exchange to figure the speed between the two points. Previous speed tests are also provided in the `previous` array.
	
![Executium Server Location Speed to Exchange Test](https://i.imgur.com/G7IwvSp.png)
	
When selecting a server to run your speed test from utilize `/api/v2/subscriptions/list-private-servers` or `/api/v2/subscriptions/list-shared-servers` as endpoints. Note that subscription restrictions may apply.
	

```
POST /api/v2/tests/server-location-speed-to-exchange
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
server_id |  | YES |  | Executium server location.
exchange1 |  | YES |  | The first exchange to ping.
exchange2 |  | YES |  | The second exchange to ping.


## Exchange Index Announcements
The exchange index service announcements.

```
GET /api/v2/exchangeindex/announcements
```

**Parameters:**
None

## Monitored Exchanges
A comprehensive list of all the exchanges which the executium exchange index monitors.

```
GET /api/v2/exchangeindex/exchanges
```

**Parameters:**
None

## Relevant News
Relevant news to a a `symbol`.  Our exchange checks news every minute of the day and matches to symbols where it is most relevant.

```
POST /api/v2/exchangeindex/relevant-news
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
symbol |  | YES |  | The executium code, which can be found at [exchanges-supported.md](./exchanges-supported.md) or by calling the endpoint `system/symbols`.


## Monitored Symbols
A comprehensive list of all the symbols which executiums exchange index monitors. This can be filtered down to exchanges.

```
POST /api/v2/exchangeindex/symbols
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
exchange |  | YES |  | 
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Export Fetch
Use the `id` provide from `export/fetch` to pull down your export request. Please note htese can take a period of time to generate. Please be patient.

```
POST /api/v2/export/fetch
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
 |  | YES | transactions | Provide the export ID you was provided from the `export/request`


## Export List
List all export requests, these are not stored indefinitely and have a limitation. Review your expiration date of any expot request to be sure.

```
POST /api/v2/export/list
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Request Export
Request an export of data to a file. Once requested you will be provided n ID where you must go to the `export/fetch` endpoint to retrieve the file. If the file is not ready it will provide a message prompting you to wait.

```
POST /api/v2/export/request
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
system |  | YES | strategy_transactions | Options: strategy_transactions, all_strategies, 
type |  | YES |  | Export Type .xls or .csv
symbol |  | YES |  | The executium code, which can be found at [exchanges-supported.md](./exchanges-supported.md) or by calling the endpoint `system/symbols`.
limit |  | YES | 100 | 


## Add Reminder


```
GET /api/v2/calendar/add-reminder
```

**Parameters:**
None

## List Schedule


```
GET /api/v2/calendar/list-schedule
```

**Parameters:**
None

## Algorithm Add


```
POST /api/v2/algorithm-creator/algorithm-add
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
name | 4 | YES |  | Provide the name of your algo.


## Algorithm Remove


```
GET /api/v2/algorithm-creator/algorithm-remove
```

**Parameters:**
None

## Algorithm Statistics


```
GET /api/v2/algorithm-creator/algorithm-statistics
```

**Parameters:**
None

## Algorithm Update


```
GET /api/v2/algorithm-creator/algorithm-update
```

**Parameters:**
None

## Condition Add


```
GET /api/v2/algorithm-creator/condition-add
```

**Parameters:**
None

## Condition Remove


```
GET /api/v2/algorithm-creator/condition-remove
```

**Parameters:**
None

## Condition Update


```
GET /api/v2/algorithm-creator/condition-update
```

**Parameters:**
None

## Execution Add


```
GET /api/v2/algorithm-creator/execution-add
```

**Parameters:**
None

## Execution Remove


```
GET /api/v2/algorithm-creator/execution-remove
```

**Parameters:**
None

## Execution Update


```
GET /api/v2/algorithm-creator/execution-update
```

**Parameters:**
None

## List Algorithms


```
GET /api/v2/algorithm-creator/list-algorithms
```

**Parameters:**
None

## List Condition Operators


```
GET /api/v2/algorithm-creator/list-condition-operators
```

**Parameters:**
None

## List Conditions


```
GET /api/v2/algorithm-creator/list-conditions
```

**Parameters:**
None

## List Executions


```
GET /api/v2/algorithm-creator/list-executions
```

**Parameters:**
None

## List Order Types


```
GET /api/v2/algorithm-creator/list-order-types
```

**Parameters:**
None

## Publish Algorithm


```
GET /api/v2/algorithm-creator/publish-algorithm
```

**Parameters:**
None

## Unpublish Algorithm


```
GET /api/v2/algorithm-creator/unpublish-algorithm
```

**Parameters:**
None

## Validate Algorithm


```
GET /api/v2/algorithm-creator/validate-algorithm
```

**Parameters:**
None

## Signal Trigger
Send your trigger conditions to this endpoint. You must send both a signal (buy or sell) and a corresponding action (open or close). This is required as a double verification prevention method.

```
POST /api/v2/marketplace/signals-trigger
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide a Signal ID
signal |  | YES |  | `buy` or `sell`. If this is the closing portion of the `signal` then you must do the opposite to what occured in the opening signal.
action |  | YES |  | Indicate if you are `open` or `close` with this signal. It must correlate to the current status. Both `signal` and `action` must exist and be correct as a confirmation that you are performing the correct actions.
execute_within |  | YES |  | Determine in milliseconds in which the window to execute the `signal`.
maximum_amount |  | YES |  | Maximum amount to buy/sell


## Edit Signal


```
POST /api/v2/marketplace/signals-edit
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide a Signal ID
name |  | NO |  | Signal Name
custom_1 |  | NO |  | Custom 1 Data
custom_2 |  | NO |  | Custom 2 Data


## Reset Signal Statistics
You must be the owner of the signal to reset the statistics. Please note, by resetting the data you will place your entire signal back to the start. All related logging data will be destroyed. This is not recommended.

```
POST /api/v2/marketplace/signal-reset
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide a Signal ID


## Signals Feed
The REST endpoint to receive signal instructions and information. We recommend using the websocket for the signal endpoint if you are intending polling. Please note that there is a delay in these signals in the `public` domain. The true speed for `signals` is only available by using the executium trading system. This endpoint is provided as a means to give delayed, yet accurate information on how a signal is performing. If you are looking to utilize these signals as part of your trading strategy then you should use the executium trading system strategy engine to leverage the signal data.

```
POST /api/v2/marketplace/signals-feed
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | NO |  | Provide a Signal ID
code |  | NO |  | Filter your results to a specific executium code
more |  | NO |  | Set to `1` or `true` to activate more `iteration_children` options. By default you will only have returned 1 row of `iteration_children` data.
limit |  | NO | 100 | Relevant to the `iteration_children` array only. 
min_iterations |  | NO |  | The minimum amount of iterations to display in the results
from_iteration |  | NO |  | Display results of signals which contain a minimum of iterations.
pagenumber |  | NO | 1 | Relevant to the `iteration_children` only.


**Successful Response Payload:**
```javascript
 "data":{
      "signals":[
         {
            "id":"1",
            "time_created":"1596609068",
            "last_updated":"1596951846788",
            "c_uid":0,
            "c_name":"Volume Creator",
            "c_status":"closed",
            "c_iteration":"4678",
            "c_profit":"-3185.01000000",
            "c_order":"0.70231753",
            "c_average":"-0.70231753",
            "c_usdt_volume":"53017671.67",
            "c_last_profit":"-4.05000000",
            "c_last_runtime":"6827",
            "c_direction":"short",
            "c_codes":"binance-btcusdt",
            "c_description":"",
            "c_price":"0.00000000",
            "c_subscribers_current":"0",
            "c_subscribers_max":"0",
            "c_success_rate":"0",
            "c_current_success_streak":"0",
            "c_action_direction_1":"sell",
            "c_action_direction_2":"buy",
            "c_action_maxtime_1":"1596951847419",
            "c_action_maxtime_2":"1596951847788",
            "c_action_maxamount_1":"0.002",
            "c_action_maxamount_2":"0.002",
            "iteration_children":[

            ]
         }
      ]
   },
```


## Create Signal Profile
Creater a signal profile for your account.

```
POST /api/v2/marketplace/signals-add
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
name | 3 | YES |  | Label your strategy
code | 3 | YES |  | Executium code only acceptable
script | 3 | YES |  | 
scriptcheck |  | NO |  | 
commissions | 1 | YES |  | 
interval | 1 | YES |  | 
position | 1 | YES |  | `long` or `short`
takeprofit | 1 | YES |  | 
takeloss | 1 | YES |  | 
datefrom | 1 | YES |  | A valid date format, example `2020-09-01`
dateto | 1 | YES |  | A valid date format, example `2020-09-01`


## Delete Signal


```
POST /api/v2/marketplace/signal-delete
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id | 1 | YES |  | Signal ID


## Signals Iteration Price Movement
The data points for an iterations ID

```
POST /api/v2/marketplace/signals-iteration-price-movement
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id | 1 | YES |  | Signal ID
iteration | 1 | YES |  | Signals Iteration ID


## Orderbook Data


```
POST /api/v2/backtesting/orderbook-data
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
exchange | 1 | YES |  | 
symbol | 1 | YES |  | Format for example `BTC/USDT`
type | 2 | YES |  | Type defaults to `spot`
timefrom | 1 | YES |  | Time from
timeto | 1 | YES |  | Time to


## Technical Indicators


```
POST /api/v2/backtesting/technical-indicators
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
exchange | 1 | YES |  | 
symbol | 1 | YES |  | Format for example `BTC/USDT`
type | 2 | YES |  | Type defaults to `spot`
interval | 1 | YES |  | `1m`, `3m`, `5m`, `15m`, `30m`, `1h`, `2h` and `4h` 
timefrom | 1 | YES |  | Time from
timeto | 1 | YES |  | Time to


## Availability Information
Information related to what is available for backtesting

```
GET /api/v2/backtesting/availability
```

**Parameters:**
None

## Create Article


```
POST /api/v2/articles/create
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
title | 18 | YES |  | A title for your work
brief | 30 | YES |  | Write an engaging article brief.
body | 300 | YES |  | The minimum length for any article must be 300 characters
publishdate | 6 | YES |  | Publish date must be measured in the number of seconds since the Unix Epoch. For example `1599615673` is `September 9th, 2020 8:41 AM`. You would submit `1599615673` as the `publishdate`
image1 |  | NO |  | Image URL 1
image2 |  | NO |  | Image URL 2
image3 |  | NO |  | Image URL 3
image4 |  | NO |  | Image URL 4
image5 |  | NO |  | Image URL 5
image6 |  | NO |  | Image URL 6


## List all of your articles
List all of your articles you have published on the platform.

```
POST /api/v2/articles/list
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
pagenumber |  | NO | 1 | 


## Delete your article
This gives you the ability to delete an article you published.

```
POST /api/v2/articles/delete
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of the article.


## Check earnings
Check all of your earnings and related statistics in one place from your publications.

```
GET /api/v2/articles/check-earnings
```

**Parameters:**
None

## Edit your article


```
POST /api/v2/articles/edit
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the article ID
title | 18 | YES |  | A title for your work
brief | 30 | YES |  | Write an engaging article brief.
body | 300 | YES |  | The minimum length for any article must be 300 characters

