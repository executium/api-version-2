# Executium Error Codes for Version 2
Errors with executium will consist of two parts within the `data` object where you can determine if the data has been returned successfully or not.

```json

 "data": {
        "code": 1440,
        "error": "Missing POST parameter(s) required to proceed, review 'missing_parameters' for more information."
    },
    
```

We then provide additional parameters to help the end user determine if they attached all required parameters

```json
   "missing_parameters": [
        "exchange",
        "label",
        "token",
        "secret"
    ], 
```

In the event they provide the parameters but they do not provide the values as expect, a `missing_information` and/or `incorrect_value_lengths` parameters will be provided. The `incorrect_value_lengths` object will highlight the name of the provided parameter which is incorrectly formatted, for example `token minimum length 5`

```json

"missing_parameters": [
    "label",
    "secret"
],
    
"missing_information": 
[
    {
        "error": "Unsupported exchange. Please review supported exchange list",
        "supported": [
            "bitfinex",
            "etc",
            "etc"
        ]
    }
],

"incorrect_value_lengths": [
    "token minimum length 5"
],

```

## Meta Object
Every request will be accompanied by `meta` data. This provides the end user valuable information about their request such as if the was  authorized or not. The `meta` data of a return requests can be a valued asset when debugging any request.

```json
    "meta": {
        "endpoint": "exchange-api-keys/add",
        "auth_required": true,
        "ms": 1591763909956,
        "time": 1591763909,
        "uid": 1,
        "process_time": "0.007602"
    }
```

## 10xx Network Issues

## 50xx Internal Issues with Executium
Any codes which fall in the 5000-6000 range are issues relating directory to the executium trading system. When you encounter these errors there is little to nothing you as a user can do. While we will be aware at the same time as you, and working towards a solution, we do request you send your request and response data to support@executium.com as this will prove helpful.




    
