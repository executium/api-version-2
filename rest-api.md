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
- Subscriptions
	- [Subscriptions Details](#subscriptions-details) (subscriptions/details)
	- [Cancel Subscription](#cancel-subscription) (subscriptions/cancel)
	- [Commissions Report](#commissions-report) (subscriptions/commissions-report)
	- [Deposit Addresses](#deposit-addresses) (subscriptions/deposit)
	- [Invoices](#invoices) (subscriptions/invoices)
	- [Change Subscription Package](#change-subscription-package) (subscriptions/change-package)
	- [Change Setting](#change-setting) (subscriptions/change-setting-request)
	- [Disable Private Server](#disable-private-server) (subscriptions/disable-private-server)
	- [Subscriptions Disable Shared Server](#subscriptions-disable-shared-server) (subscriptions/disable-shared-server)
	- [Enable Private Server](#enable-private-server) (subscriptions/enable-private-server)
	- [Enable Shared Server](#enable-shared-server) (subscriptions/enable-shared-server)
	- [List Private Servers](#list-private-servers) (subscriptions/list-private-servers)
	- [List Shared Servers](#list-shared-servers) (subscriptions/list-shared-servers)
	- [Package Recommendation](#package-recommendation) (subscriptions/package-recommendation)
	- [Commissions Rate](#commissions-rate) (subscriptions/commissions-rate)
	- [Subscriptions List Packages](#subscriptions-list-packages) (subscriptions/list-packages)
	- [Subscriptions Change Setting Confirm](#subscriptions-change-setting-confirm) (subscriptions/change-setting-confirm)
	- [Subscriptions Server Types](#subscriptions-server-types) (subscriptions/server-types)
- Exchange Api Keys
	- [Add Exchange API Credentials](#add-exchange-api-credentials) (exchange-api-keys/add)
	- [Delete Exchange API Key](#delete-exchange-api-key) (exchange-api-keys/delete)
	- [List Exchange API Keys](#list-exchange-api-keys) (exchange-api-keys/list)
	- [Check Specific Exchange Symbol Balance ](#check-specific-exchange-symbol-balance-) (exchange-api-keys/check-balances)
- Strategy
	- [Create New Strategy](#create-new-strategy) (strategy/create)
	- [Strategy High Level Overview](#strategy-high-level-overview) (strategy/high-level-overview)
	- [User Strategy List](#user-strategy-list) (strategy/data/list)
	- [List All Trading Algorithms](#list-all-trading-algorithms) (strategy/list-algorithms)
	- [Exchange List](#exchange-list) (strategy/list-exchanges)
	- [Debug Data](#debug-data) (strategy/data/debug)
	- [Save Template](#save-template) (strategy/save-template)
	- [Strategy List Templates](#strategy-list-templates) (strategy/list-templates)
	- [Strategy Start](#strategy-start) (strategy/start)
	- [Strategy Stop](#strategy-stop) (strategy/stop)
	- [List Active Strategies](#list-active-strategies) (strategy/list-active-strategies)
	- [List Strategy Transactions](#list-strategy-transactions) (strategy/list-strategy-transactions)
	- [Stop All Strategies](#stop-all-strategies) (strategy/stop-all-strategies)
	- [Strategy Update](#strategy-update) (strategy/update)
	- [List Strategy Options](#list-strategy-options) (strategy/list-strategy-options)
- Public
	- [Spreads](#spreads) (public/spreads/data)
	- [Fetch Symbol Price](#fetch-symbol-price) (public/fetch-symbol-price)
	- [Bitcoin Price Tracker](#bitcoin-price-tracker) (public/bitcoin-price-tracker)
	- [Fetch Symbol Trades](#fetch-symbol-trades) (public/fetch-symbol-trades)
	- [Realtime Bitcoin Profit](#realtime-bitcoin-profit) (public/realtime-bitcoin-profit)
	- [Exchange Information](#exchange-information) (public/exchange-information)
	- [Tradingview Charts](#tradingview-charts) (public/tradingview-charts)
- Subaccounts
	- [Create Sub Account](#create-sub-account) (subaccounts/subaccount-create)
	- [List All Subaccounts](#list-all-subaccounts) (subaccounts/subaccount-list)
	- [Delete Subaccount](#delete-subaccount) (subaccounts/subaccount-delete)
	- [Edit Subaccount](#edit-subaccount) (subaccounts/subaccount-edit)
	- [Send Broadcast](#send-broadcast) (subaccounts/broadcast-create)
	- [Delete Broadcast](#delete-broadcast) (subaccounts/broadcast-delete)
	- [Edit Broadcast](#edit-broadcast) (subaccounts/broadcast-edit)
	- [List Broadcast](#list-broadcast) (subaccounts/broadcast-list)
	- [Subaccounts Subaccount Access History](#subaccounts-subaccount-access-history) (subaccounts/subaccount-access-history)
- User
	- [Close Account](#close-account) (user/close-account)
	- [User Account Balance](#user-account-balance) (user/account-balance)
	- [User Access History](#user-access-history) (user/access-history)
	- [User Account Details](#user-account-details) (user/account-details)
	- [User List Referrals](#user-list-referrals) (user/list-referrals)
	- [User Active Sessions](#user-active-sessions) (user/active-sessions)
	- [User Security Settings](#user-security-settings) (user/security-settings)
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
	- [Finance Import Orders List](#finance-import-orders-list) (finance/import-orders-list)
	- [Finance Import Orders Settings](#finance-import-orders-settings) (finance/import-orders-settings)
- Exchange API Keys
	- [Test API Key Status](#test-api-key-status) (exchange-api-keys/test)
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
	- [Calendar Add Reminder](#calendar-add-reminder) (calendar/add-reminder)
	- [Calendar List Schedule](#calendar-list-schedule) (calendar/list-schedule)
- Exchange Query
	- [Exchange Query List Balances](#exchange-query-list-balances) (exchange-query/list-balances)
	- [Exchange Query List Closed Orders](#exchange-query-list-closed-orders) (exchange-query/list-closed-orders)
	- [Exchange Query List Open Orders](#exchange-query-list-open-orders) (exchange-query/list-open-orders)


# Public REST API Version 2 for Executium (private beta)

## Accessibility
Currently executium version 2 is in private beta mode as of 10th June 2020. We will update the status of the public release date in this file when decided upon.

## General Information

* Version 2 is currently in private beta.
* The base endpoint is: **`[CLOSED-BETA-VERSION]`**
* All endpoints return either a JSON object or array.
* There are currently **`94 endpoints`** as part of version 2.
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
All symbols listed and supported on executium. 

```
GET /api/v2/system/symbols
```

**Parameters:**
None

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
page |  | NO | 1 | 


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
Provide the ID of the package you wish to change your current subscription too. You can find the packages `id` via the `subscription/list-packages` endpoint.

```
POST /api/v2/subscriptions/change-package
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of package you wish to change too.


## Change Setting
You can change individual settings of a subscription to have more or less of something. Once you make a change your package will become `custom`. When you request a change you will be provided with a subscription price adjustment `id`.  Use this provided ID with the endpoint `subscriptions/change-setting-confirm`

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
List all the private servers your currently have on your package.

```
POST /api/v2/subscriptions/list-private-servers
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
page |  | NO | 1 | 


## List Shared Servers
List all shared servers currently available to you. These will also include those as defaulted to you by your subscription package. When you join any subscription, even the free tier of executium, you are nominated servers for your strategies to run on. These provided servers are inclusive of your subscription cost and subject to change by the hour. They will not change if you have an existing strategy running on them.

```
POST /api/v2/subscriptions/list-shared-servers
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
page |  | NO | 1 | 


## Package Recommendation
Based on an array of inputs we will provide a recommended package for you.

```
GET /api/v2/subscriptions/package-recommendation
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

## Subscriptions List Packages


```
GET /api/v2/subscriptions/list-packages
```

**Parameters:**
None

## Subscriptions Change Setting Confirm


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


## Delete Exchange API Key
Delete a Exchange API Key from your account. In the event that the key is being used by a running strategy you will not be able to remove the key until that has been stopped.

```
POST /api/v2/exchange-api-keys/delete
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of the key you wish to remove.


## List Exchange API Keys
A full list of accessible Exchange API Keys in your account. This will not show the API keys secrets. If a subaccount user is accessing the API key list they will only see according to their permissions.

```
POST /api/v2/exchange-api-keys/list
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
page |  | NO | 1 | 


## Check Specific Exchange Symbol Balance 
Functions in a similar fashion to `list-balances`.

```
GET /api/v2/exchange-api-keys/check-balances
```

**Parameters:**
None

## Create New Strategy
Create a new strategy, you will be required to make additional modifications using other endpoints such as the algo selector and updating the information within.

```
POST /api/v2/strategy/create
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
label | 6 | YES |  | 
algo |  | YES |  | 


**Successful Response Formatted:**

Name | Example Value
------------ | ------------
status | 1
id | See table 'Id'
uid | 1
label | Example of a strategy label
message | New - Testing Credentials


### Id

Name | Example Value
------------ | ------------


**Successful Response Payload:**
```javascript
{
    "data": {
        "status": true,
        "id": [],
        "uid": "1",
        "label": "Example of a strategy label",
        "message": "New - Testing Credentials"
    },
    "meta": {
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
        "endpoint": "strategy/create",
        "auth_required": true,
        "ms": 1591778250176,
        "time": 1591778250,
        "uid": 1,
        "process_time": "0.020210"
    }
}
```


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
page |  | NO | 1 | 


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
You must specifically call a strategy start event using this endpoint. If you execute this endpoint while a strategy is running nothing will happen.

```
GET /api/v2/strategy/start
```

**Parameters:**
None

## Strategy Stop
This endpoint is to specifically tell the strategy to stop. When it has been executed it will attempt to clean up and cancel any pending orders before it fully stops. This can take an unspecified period of time to complete as the system works to confirm that anything pending is completed. You can consult the `force` parameter for a hard stop.

```
POST /api/v2/strategy/stop
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
force |  | NO |  | If you select to force the stop it will stop immediately and not check to see if the orders are still active at the exchanges. In the event this parameter is used you must cancel the orders yourself via the exchange(s). In the event you start the strategy after a forced stop, the strategy format will reconvene and check any pending orders.


## List Active Strategies
A complete list of strategies that are actively running on executium.

```
GET /api/v2/strategy/list-active-strategies
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
page |  | NO | 1 | 
main_id |  | YES |  | 
leg_id |  | YES |  | 


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

## Spreads
Data which is served in a public manner and is obtainable via a public call. Additional restrictions may apply and tighter rate limiting. To upgrade your account for faster access please visit executium.

```
GET /api/v2/public/spreads/data
```

**Parameters:**
None

## Fetch Symbol Price
Public API but restrictions apply based on your subscription level. You must provide the exact `symbol` code which executium provides. You can review symbols in the `system/symbols` endpoint.

```
POST /api/v2/public/fetch-symbol-price
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
symbol |  | YES |  | The executium code, which can be found at [exchanges-supported.md](./exchanges-supported.md) or by calling the endpoint `system/symbols`.
side |  | YES |  | Choice: 'asks' or 'bids'; If you input 'buy' it will show 'asks'; If you input 'sell' it will show 'bids'; No other inputs will be accepted.
level |  | YES | 1 | The orderbook level, from 1 to 10


## Bitcoin Price Tracker
Data related to the current price of Bitcoin in realtime. This endpoint only provides the data streams. You should use your own graph product to map the data. A minimum of 1 exchange is required to run and a maximum of 6 is possible.

```
POST /api/v2/public/bitcoin-price-tracker
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
exchange1 |  | YES |  | 
exchange2 |  | NO |  | 
exchange3 |  | NO |  | 
exchange4 |  | NO |  | 
exchange5 |  | NO |  | 
exchange6 |  | NO |  | 


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
page |  | NO | 1 | 


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
parent_maximum |  | YES | 0.1 | Maximum parent in BTC that the subaccount can place per strategy
child_maximum |  | YES | 0.01 | Maximum child in BTC that the subaccount can place per strategy
exchanges_enabled |  | YES | All | Select which exchanges the subaccount has access too for strategy management.
concurrent_strategies_maximum |  | YES |  | The amount of strategies that the subaccount can run concurrently.
export_enabled |  | YES |  | The subaccount ability to export data (true/true)
share_accounts_apikeys |  | YES |  | Allow or deny the subaccount to have access to all of the keys in the account (true/true).
manage_own_apikeys |  | YES |  | Provide the subaccount the ability to manage their own api keys (true/true).
force_twofactor |  | YES |  | Force the subaccount to setup two factor on their account (true/true)
allow_api_access |  | YES |  | Allow or deny the subaccount access to the account API, in the event the account is given access new API keys for the subaccount will need to be generated (true/true).


## List All Subaccounts
Available in subscrition packages. View ID and subaccount information.

```
GET /api/v2/subaccounts/subaccount-list
```

**Parameters:**
None

## Delete Subaccount
You can delete any subaccount by providing the ID, which can be obtain by `list-subaccount`. When you delete a subaccount it will not remove any other related information such as `strategy` or `history`. All information will still eist with the primary account holder.

```
GET /api/v2/subaccounts/subaccount-delete
```

**Parameters:**
None

## Edit Subaccount
You can edit all basic features about a subaccount but not the `password` or `active status` through the API. To change a subaccount password you must login to the website. If you wish to disable an account use the `subaccounts/subaccount-delete` endpoint,

```
GET /api/v2/subaccounts/subaccount-edit
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
page |  | NO | 1 | 


## Subaccounts Subaccount Access History


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
page |  | NO | 1 | 


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
page |  | NO | 1 | 


## User Active Sessions
Show all of your current active sessions which are logged into the web system.

```
GET /api/v2/user/active-sessions
```

**Parameters:**
None

## User Security Settings
List all of your security settings and current configuration. These settings apply to your subaccounts also.

```
GET /api/v2/user/security-settings
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
type |  | YES | BTC | 


## Wallets List Balances
List all wallets related to your account for direct purpose of depositing subscription and commission fees too.

```
GET /api/v2/wallets/list-balances
```

**Parameters:**
None

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
page |  | NO | 1 | 


## List Recent Transactions
List all of your most recent transactions related to your executium. This includes your subscription and commissions costs.

```
POST /api/v2/finance/list-recent-transactions
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
page |  | NO | 1 | 


## List Top Strategy PNL
List all of your most recent strategies and their related profit and loss .

```
POST /api/v2/finance/list-top-strategy-pnl
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
page |  | NO | 1 | 


## List Deposits
List deposits which have come into executium. This is the deposits which have been made to pay for subscription and commission fees.

```
POST /api/v2/finance/list-depoists
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
page |  | NO | 1 | 


## List Withdraws
See `wallets/withdraw`

```
GET /api/v2/finance/list-withdraws
```

**Parameters:**
None

## Finance Import Orders List


```
GET /api/v2/finance/import-orders-list
```

**Parameters:**
None

## Finance Import Orders Settings


```
GET /api/v2/finance/import-orders-settings
```

**Parameters:**
None

## Test API Key Status
You must use the returned `id` for the keys you wish to test. From this we will run a test to determine if the keys are valid. If they are tested to be invalid then they will also be disabled for selection system-wide.

```
POST /api/v2/exchange-api-keys/test
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide ID of the API key from `exchange-api-keys/list`


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
page |  | NO | 1 | 


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
page |  | NO | 1 | 


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


## Calendar Add Reminder


```
GET /api/v2/calendar/add-reminder
```

**Parameters:**
None

## Calendar List Schedule


```
GET /api/v2/calendar/list-schedule
```

**Parameters:**
None

## Exchange Query List Balances


```
GET /api/v2/exchange-query/list-balances
```

**Parameters:**
None

## Exchange Query List Closed Orders


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
