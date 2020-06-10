# Executium Error Codes for Version 2
Errors with executium will consist of two parts within the `data` object where you can determine if the data has been returned successfully or not.

```json

 "data": {
        "code": 1440,
        "error": "Missing POST parameter(s) required to proceed, review 'missing_parameters' for more information. "
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


    
