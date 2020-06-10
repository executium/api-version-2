


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
- Subscriptions
	- [Subscription Detail](#subscription-detail) (subscriptions/details)
	- [Cancel](#cancel) (subscriptions/cancel)
	- [Commissions Report](#commissions-report) (subscriptions/commissions-report)
	- [Deposit](#deposit) (subscriptions/deposit)
	- [Invoices](#invoices) (subscriptions/invoices)
- Exchange Api Keys
	- [Add Exchange API Credentials](#add-exchange-api-credentials) (exchange-api-keys/add)
	- [Delete](#delete) (exchange-api-keys/delete)
	- [List](#list) (exchange-api-keys/list)
- Strategy
	- [Create New Strategy](#create-new-strategy) (strategy/create)
	- [User Strategy Overview](#user-strategy-overview) (strategy/data/all)
	- [User Strategy List](#user-strategy-list) (strategy/data/list)
	- [Trading Algorithms](#trading-algorithms) (strategy/list-algorithms)
	- [Exchange List](#exchange-list) (strategy/list-exchanges)
	- [Data](#data) (strategy/data/debug)
	- [Save Template](#save-template) (strategy/save-template)
- Public
	- [Spreads](#spreads) (public/spreads/data)
- Subaccounts
	- [Create](#create) (subaccounts/create)
	- [List](#list) (subaccounts/list)
	- [Delete](#delete) (subaccounts/delete)
	- [Edit](#edit) (subaccounts/edit)
- User
	- [Close Account](#close-account) (user/close-account)


# Public REST API Version 2 for Executium (private beta)

## Accessibility
Currently executium version 2 is in private beta mode as of 10th June 2020. We will update the status of the public release date in this file when decided upon.

## General Information

* Version 2 is currently in private beta.
* The base endpoint is: **[CLOSED-BETA-VERSION]**
* All endpoints return either a JSON object or array.
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

## Endpoints
A list of all the available endpoints.

```
GET /api/v2/system/endpoints
```

**Parameters:**
None

## Ping REST API
Text the connectivity to the REST API

```
GET /api/v2/system/ping
```

**Parameters:**
Name | MinLength | Required | Default | Description
------------ | ------------ | ------------ | ------------ | ------------
milliseconds | 0 | NO | 0 | Provide a milliseconds timestamp and then the server will provide a subtracted return value from your input. For more information about millisecond functions visit https://github.com/executium/millisecond-functions


**Successful Response:**
```javascript
{
  \"data\": {
    \"our_server_ms\": 1591777804071,
    \"your_sent_ms\": \"1591777804158\",
    \"difference\": -87,
    \"equation\": \"our_server_ms - your_sent_ms\",
    \"note\": \"Always make sure your devices time is synchronized for best results.\"
  },
  \"meta\": {
    \"api_version\": 2,
    \"system_version\": \"2.0.5\",
    \"status\": 200,
    \"endpoint\": \"system/ping\",
    \"auth_required\": false,
    \"ms\": 1591777804071,
    \"time\": 1591777804,
    \"uid\": -1,
    \"process_time\": \"0.000204\"
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

## Subscription Detail
A breakdown on your current subscription with executium. The subscription details provide a full insight into all components of your subscription plan.

```
GET /api/v2/subscriptions/details
```

**Parameters:**
None

## Cancel


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

## Deposit


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
exchange | 0 | YES |  | See the supported exchanges via the `strategy/list-exchanges` endpoint
label | 6 | YES |  | Label the 
token | 5 | YES |  | API key/token
secret | 4 | YES |  | API secret
password | 0 | NO |  | Some exchanges, such as OKEx require a password to be provided.


## Delete


```
GET /api/v2/exchange-api-keys/delete
```

**Parameters:**
None

## List


```
GET /api/v2/exchange-api-keys/list
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
algo | 0 | YES |  | 


**Successful Response:**
```javascript
{
    \"data\": {
        \"status\": true,
        \"id\": [],
        \"uid\": \"1\",
        \"label\": \"Example of a strategy label\",
        \"message\": \"New - Testing Credentials\"
    },
    \"meta\": {
        \"api_version\": 2,
        \"system_version\": \"2.0.5\",
        \"status\": 200,
        \"auth_success\": true,
        \"rateLimits\": {
            \"minute\": 60
        },
        \"subscription\": {
            \"id\": \"0\",
            \"name\": \"Free\"
        },
        \"endpoint\": \"strategy/create\",
        \"auth_required\": true,
        \"ms\": 1591778250176,
        \"time\": 1591778250,
        \"uid\": 1,
        \"process_time\": \"0.020210\"
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
limit | 0 | NO | 10 | 
page | 0 | NO | 1 | 


## Trading Algorithms
A full list of executium trading algorithms. You will be required to reference your subscription to understand which algorithms are available for usage for you on your current strategy.

```
GET /api/v2/strategy/list-algorithms
```

**Parameters:**
None

## Exchange List
A full list of exchanges that excutium support

```
GET /api/v2/strategy/list-exchanges
```

**Parameters:**
None

## Data


```
GET /api/v2/strategy/data/debug
```

**Parameters:**
None

## Save Template


```
GET /api/v2/strategy/save-template
```

**Parameters:**
None

## Spreads


```
GET /api/v2/public/spreads/data
```

**Parameters:**
None

## Create


```
GET /api/v2/subaccounts/create
```

**Parameters:**
None

## List


```
GET /api/v2/subaccounts/list
```

**Parameters:**
None

## Delete


```
GET /api/v2/subaccounts/delete
```

**Parameters:**
None

## Edit


```
GET /api/v2/subaccounts/edit
```

**Parameters:**
None

## Close Account


```
GET /api/v2/user/close-account
```

**Parameters:**
None
