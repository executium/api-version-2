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
- Subscriptions
	- [Subscription Detail](#subscription-detail) (subscriptions/details)
- Exchange API Keys
	- [Add Exchange API Credentials](#add-exchange-api-credentials) (exchange-api-keys/add)
- Strategy
	- [Create New Strategy](#create-new-strategy) (strategy/create)
	- [User Strategy Overview](#user-strategy-overview) (strategy/data/all)
	- [User Strategy List](#user-strategy-list) (strategy/data/list)
	- [Trading Algorithms](#trading-algorithms) (strategy/list-algorithms)
	- [Exchange List](#exchange-list) (strategy/list-exchanges)


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

## Endpoints

## Ping REST API

## Subscription Detail

## Add Exchange API Credentials

## Create New Strategy

## User Strategy Overview

## User Strategy List

## Trading Algorithms

## Exchange List
