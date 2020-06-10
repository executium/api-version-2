
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
	- [Subscription Detail](#subscription-detail) (subscriptions/details)
	- [Cancel Subscription](#cancel-subscription) (subscriptions/cancel)
	- [Commissions Report](#commissions-report) (subscriptions/commissions-report)
	- [Deposit Addresses](#deposit-addresses) (subscriptions/deposit)
	- [Invoices](#invoices) (subscriptions/invoices)
- Exchange Api Keys
	- [Add Exchange API Credentials](#add-exchange-api-credentials) (exchange-api-keys/add)
	- [Delete Exchange API Key](#delete-exchange-api-key) (exchange-api-keys/delete)
	- [List Exchange API Keys](#list-exchange-api-keys) (exchange-api-keys/list)
	- [Exchange Api Keys Check Balances](#exchange-api-keys-check-balances) (exchange-api-keys/check-balances)
	- [Exchange Api Keys Test](#exchange-api-keys-test) (exchange-api-keys/test)
- Strategy
	- [Create New Strategy](#create-new-strategy) (strategy/create)
	- [User Strategy Overview](#user-strategy-overview) (strategy/data/all)
	- [User Strategy List](#user-strategy-list) (strategy/data/list)
	- [List All Trading Algorithms](#list-all-trading-algorithms) (strategy/list-algorithms)
	- [Exchange List](#exchange-list) (strategy/list-exchanges)
	- [Debug Data](#debug-data) (strategy/data/debug)
	- [Save Template](#save-template) (strategy/save-template)
	- [Strategy List Templates](#strategy-list-templates) (strategy/list-templates)
	- [Strategy Start](#strategy-start) (strategy/start)
	- [Strategy Stop](#strategy-stop) (strategy/stop)
	- [Strategy List Active Strategies](#strategy-list-active-strategies) (strategy/list-active-strategies)
	- [Strategy List Strategy Transactions](#strategy-list-strategy-transactions) (strategy/list-strategy-transactions)
	- [Strategy Stop All Strategies](#strategy-stop-all-strategies) (strategy/stop-all-strategies)
	- [Strategy Update](#strategy-update) (strategy/update)
- Public
	- [Spreads](#spreads) (public/spreads/data)
	- [Fetch Symbol Price](#fetch-symbol-price) (public/fetch-symbol-price)
	- [Public Bitcoin Price Tracker](#public-bitcoin-price-tracker) (public/bitcoin-price-tracker)
	- [Public Fetch Symbol Trades](#public-fetch-symbol-trades) (public/fetch-symbol-trades)
	- [Public Realtime Bitcoin Profit](#public-realtime-bitcoin-profit) (public/realtime-bitcoin-profit)
	- [Public Exchange Information](#public-exchange-information) (public/exchange-information)
- Subaccounts
	- [Create Subaccount](#create-subaccount) (subaccounts/create)
	- [List All Subaccounts](#list-all-subaccounts) (subaccounts/list)
	- [Delete Subaccount](#delete-subaccount) (subaccounts/delete)
	- [Edit Subaccount](#edit-subaccount) (subaccounts/edit)
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
	- [Wallets Withdraw](#wallets-withdraw) (wallets/withdraw)
- Finance
	- [Finance List Commissions Paid](#finance-list-commissions-paid) (finance/list-commissions-paid)
	- [Finance List Recent Transactions](#finance-list-recent-transactions) (finance/list-recent-transactions)
	- [Finance List Top Strategy Pnl](#finance-list-top-strategy-pnl) (finance/list-top-strategy-pnl)
	- [Finance List Depoists](#finance-list-depoists) (finance/list-depoists)
	- [Finance List Withdraws](#finance-list-withdraws) (finance/list-withdraws)
- Tests
	- [Black Scholes Calculator](#black-scholes-calculator) (tests/black-scholes-calculator)
	- [Black Scholes Implied Volatility Calculator](#black-scholes-implied-volatility-calculator) (tests/black-scholes-implied-volatility-calculator)


# Public REST API Version 2 for Executium (private beta)

## Accessibility
Currently executium version 2 is in private beta mode as of 10th June 2020. We will update the status of the public release date in this file when decided upon.

## General Information

* Version 2 is currently in private beta.
* The base endpoint is: **[CLOSED-BETA-VERSION]**
* All endpoints return either a JSON object or array.
* There are currently 59 endpoints as part of version 2.
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

**Successful Response:**
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

**Successful Response:**
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
GET /api/v2/system/ping
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
milliseconds |  | NO | 0 | Provide a milliseconds timestamp and then the server will provide a subtracted return value from your input. For more information about millisecond functions visit https://github.com/executium/millisecond-functions


**Successful Response:**
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


```
GET /api/v2/system/information
```

**Parameters:**
None

## List Validation Functions


```
GET /api/v2/system/list-validation-functions
```

**Parameters:**
None

## Symbols


```
GET /api/v2/system/symbols
```

**Parameters:**
None

## System Status


```
GET /api/v2/system/status
```

**Parameters:**
None

## List Announcements


```
GET /api/v2/system/list-announcements
```

**Parameters:**
None

## Subscription Detail
A breakdown on your current subscription with executium. The subscription details provide a full insight into all components of your subscription plan.

```
GET /api/v2/subscriptions/details
```

**Parameters:**
None

## Cancel Subscription


```
GET /api/v2/subscriptions/cancel
```

**Parameters:**
None

## Commissions Report


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


```
GET /api/v2/subscriptions/invoices
```

**Parameters:**
None

## Add Exchange API Credentials
Provide Exchange API credentials for usage with your executium strategies. Once added they will be confirmed and then be made available to strategies.

```
GET /api/v2/exchange-api-keys/add
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
exchange |  | YES |  | See the supported exchanges via the `strategy/list-exchanges` endpoint
label | 6 | YES |  | The label will appear when selecting your API keys for strategies. 
token | 5 | YES |  | API key/token
secret | 4 | YES |  | API secret
password |  | NO |  | Some exchanges, such as OKEx require a password to be provided.


## Delete Exchange API Key
Delete a Exchange API Key from your account. In the event that the key is being used by a running strategy you will not be able to remove the key until that has been stopped.

```
GET /api/v2/exchange-api-keys/delete
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
id |  | YES |  | Provide the ID of the key you wish to remove.


## List Exchange API Keys
A full list of accessible Exchange API Keys in your account. This will not show the API keys secrets. If a subaccount user is accessing the API key list they will only see according to their permissions.

```
GET /api/v2/exchange-api-keys/list
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
limit |  | NO | 10 | 
page |  | NO | 1 | 


## Exchange Api Keys Check Balances


```
GET /api/v2/exchange-api-keys/check-balances
```

**Parameters:**
None

## Exchange Api Keys Test


```
GET /api/v2/exchange-api-keys/test
```

**Parameters:**
None

## Create New Strategy
Create a new strategy, you will be required to make additional modifications using other endpoints such as the algo selector and updating the information within.

```
GET /api/v2/strategy/create
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
label | 6 | YES |  | 
algo |  | YES |  | 


**Successful Response:**
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


## User Strategy Overview
A compiled list of the users strategies. This data includes what is currently active, inactive and all totals related.

```
GET /api/v2/strategy/data/all
```

**Parameters:**
None

## User Strategy List
A complete list of user created strategies

```
GET /api/v2/strategy/data/list
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

**Successful Response:**
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
GET /api/v2/strategy/save-template
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
copy_strategy_id |  | YES |  | Provide the strategy ID you would like to save as a template.
label |  | NO |  | Optional field. If left blank or not provided the strategy template will be saved as the strategy name.


## Strategy List Templates


```
GET /api/v2/strategy/list-templates
```

**Parameters:**
None

## Strategy Start


```
GET /api/v2/strategy/start
```

**Parameters:**
None

## Strategy Stop


```
GET /api/v2/strategy/stop
```

**Parameters:**
None

## Strategy List Active Strategies


```
GET /api/v2/strategy/list-active-strategies
```

**Parameters:**
None

## Strategy List Strategy Transactions


```
GET /api/v2/strategy/list-strategy-transactions
```

**Parameters:**
None

## Strategy Stop All Strategies


```
GET /api/v2/strategy/stop-all-strategies
```

**Parameters:**
None

## Strategy Update
Strategies can only be updated when they are stopped. If the strategy is active the update attempt will not be processed.

```
GET /api/v2/strategy/update
```

**Parameters:**
None

## Spreads


```
GET /api/v2/public/spreads/data
```

**Parameters:**
None

## Fetch Symbol Price


```
GET /api/v2/public/fetch-symbol-price
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
symbol |  | YES |  | The executium code, which can be found at [exchanges-supported.md](./exchanges-supported.md) or by calling the endpoint `system/symbols`.
side |  | YES |  | Choice: 'asks' or 'bids'; If you input 'buy' it will show 'asks'; If you input 'sell' it will show 'bids'; No other inputs will be accepted.
level |  | NO | 1 | The orderbook level, from 1 to 10


## Public Bitcoin Price Tracker


```
GET /api/v2/public/bitcoin-price-tracker
```

**Parameters:**
None

## Public Fetch Symbol Trades


```
GET /api/v2/public/fetch-symbol-trades
```

**Parameters:**
None

## Public Realtime Bitcoin Profit


```
GET /api/v2/public/realtime-bitcoin-profit
```

**Parameters:**
None

## Public Exchange Information


```
GET /api/v2/public/exchange-information
```

**Parameters:**
None

## Create Subaccount
The primary account holder can manage inline with their subscription how many subaccounts can access/create/interact with strategies on their account.

```
GET /api/v2/subaccounts/create
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
export_enabled |  | YES |  | The subaccount ability to export data (true/false)
share_accounts_apikeys |  | YES |  | Allow or deny the subaccount to have access to all of the keys in the account (true/false).
manage_own_apikeys |  | YES |  | Provide the subaccount the ability to manage their own api keys (true/false).
force_twofactor |  | YES |  | Force the subaccount to setup two factor on their account (true/false)
allow_api_access |  | YES |  | Allow or deny the subaccount access to the account API, in the event the account is given access new API keys for the subaccount will need to be generated (true/false).


## List All Subaccounts


```
GET /api/v2/subaccounts/list
```

**Parameters:**
None

## Delete Subaccount


```
GET /api/v2/subaccounts/delete
```

**Parameters:**
None

## Edit Subaccount


```
GET /api/v2/subaccounts/edit
```

**Parameters:**
None

## Close Account
If you wish to close your account with executium this is the endpoint. We may require that you close your account via the website.

```
GET /api/v2/user/close-account
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
reason | 10 | YES |  | Please provide feedback and the reasoning for closing your account.
password | 5 | YES |  | Provide your account password.


**Successful Response:**
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


```
GET /api/v2/user/account-balance
```

**Parameters:**
None

## User Access History


```
GET /api/v2/user/access-history
```

**Parameters:**
None

## User Account Details


```
GET /api/v2/user/account-details
```

**Parameters:**
None

## User List Referrals


```
GET /api/v2/user/list-referrals
```

**Parameters:**
None

## User Active Sessions


```
GET /api/v2/user/active-sessions
```

**Parameters:**
None

## User Security Settings


```
GET /api/v2/user/security-settings
```

**Parameters:**
None

## Wallets Fetch Deposit Address


```
GET /api/v2/wallets/fetch-deposit-address
```

**Parameters:**
None

## Wallets List Balances


```
GET /api/v2/wallets/list-balances
```

**Parameters:**
None

## Wallets Withdraw


```
GET /api/v2/wallets/withdraw
```

**Parameters:**
None

## Finance List Commissions Paid


```
GET /api/v2/finance/list-commissions-paid
```

**Parameters:**
None

## Finance List Recent Transactions


```
GET /api/v2/finance/list-recent-transactions
```

**Parameters:**
None

## Finance List Top Strategy Pnl


```
GET /api/v2/finance/list-top-strategy-pnl
```

**Parameters:**
None

## Finance List Depoists


```
GET /api/v2/finance/list-depoists
```

**Parameters:**
None

## Finance List Withdraws


```
GET /api/v2/finance/list-withdraws
```

**Parameters:**
None

## Black Scholes Calculator


```
GET /api/v2/tests/black-scholes-calculator
```

**Parameters:**
None

## Black Scholes Implied Volatility Calculator


```
GET /api/v2/tests/black-scholes-implied-volatility-calculator
```

**Parameters:**
None
