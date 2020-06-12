# Executium Error Codes for Version 2
Errors with executium will consist of two parts within the `data` object where you can determine if the data has been returned successfully or not.

```javascript

 "data": {
        "code": 1440,
        "error": "Missing POST parameter(s) required to proceed, review 'missing_parameters' for more information."
    },
    
```

We then provide additional parameters to help the end user determine if they attached all required parameters

```javascript
   "missing_parameters": [
        "exchange",
        "label",
        "token",
        "secret"
    ], 
```

In the event they provide the parameters but they do not provide the values as expect, a `missing_information` and/or `incorrect_value_lengths` parameters will be provided. The `incorrect_value_lengths` object will highlight the name of the provided parameter which is incorrectly formatted, for example `token minimum length 5`

```javascript

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

```javascript
    "meta": {
        "endpoint": "exchange-api-keys/add",
        "auth_required": true,
        "ms": 1591763909956,
        "time": 1591763909,
        "uid": 1,
	"status":422,
        "process_time": "0.007602"
    }
```

## 10xx Network Issues
All codes in the 1000 to 1999 range relate to network issues.

#### 1500 - IP banned due to ignoring ratelimit
- IP banned due to repeated requests following information that the sender has been violating the ratelimits of their account.  The IP ban will stay in effect at the discretion of the system.

#### 1507 - Rate Limited By Authorization
- You are sending to many requests. You can increase your allowance by consulting your executium subscription and upgrading to a higher tier.

```javascript
    "data": {
        "code": 1507,
        "error": "Ratelimit. Next access allowable at 1591765010484. Limit set to 1 request per 1000ms"
    },
```   

#### 1508 - Rate Limited Firewall
- You are sending to many requests and being blocked at a firewall level

```javascript

    "data": {
        "code": 1508,
        "error": "Ratelimited. Please allow 0 second(s) before your next request."
    },

```   

#### 1509 - Rate Limited and Temporary IP Ban at the Firewall Level 
- Due to repeated requests to slow down your rate of request you have been automcatically banned for a specified period. Repeated violations can result in a permanent account or IP ban and will be reviewed on a case by case basis.

```javascript
    "data": {
        "code": 1509,
        "error": "Ratelimited. Extended ban applied. Please allow 59 second(s) before your next request."
    },
```   

#### 1820 - Unprocessable Entity
The `authorization` parameters sent as part of the header has malformed. This means it cannot be read so we cannot determine your API `secret` and the attached payload.

## 20xx User Input Issues
Codes within the range of 2000-2999 relate to user input errors, these can range from missing fields, illegal characters, or authorization problems.

#### 2000 - API Key invalid
- The provided API Key, parameter `key` was not valid. 

#### 2001 - Missing API Key
- The API key parameter named `key` was not present. This must be sent as part of the header.

#### 2010 - Nonce Missing from Payload
- The payload was missing the parameter `nonce`. This must be sent as part of the header.

```javascript
"data": {
        "code": 2010,
        "error": "Nonce missing"
    },
```

#### 2011 - Nonce too small
- The parameter `nonce` was present in the header, but it was a lower value than the previous sent. You must send a `nonce` value which is higher than the previous. Nonces are treated sequentially. 

```javascript
"data": {
        "code": 2011,
        "error": "Nonce too small"
    },
```

#### 2100 - Missing Authorization String
- The `authorization` parameter was not present, you are required to send this as a header.

#### 2300 - Missing required information to proceed
- Review the provided feedback objects, you have issues relating to malformed inputs. Review if present `missing_parameters`, `incorrect_value_lengths` and/or `missing_information`. These will be part of the payload returned and can be used as a pointer related to what information you have to address.

#### 2500 - Unknown Endpoint
- You provided an invalid endpoint that we do not support

## 50xx Internal Issues with Executium
Any codes which fall in the 5000-5999 range are issues relating directory to the executium trading system. When you encounter these errors there is little to nothing you as a user can do. While we will be aware at the same time as you, and working towards a solution, we do request you send your request and response data to support@executium.com as this will prove helpful.

#### 5000 - Internal database error
- An issue with the executium core engine has occured, the service will be unavilable for you on that particular request until an engineer has provided a fix.

#### 5100 - Empty End point data
- You requested an endpoint the server matched but did not pipe as expected. In this extrmeley rare/ near impossible event please contact support@executium.com

## Unable to authorize with the executium version 2 API
If you are unable to authorize we recommend you use our `php-api-sdk` for closer inspection where you can dig deeper into how we manage headers. The following messages will provide some potential help if you are having issues authorizing.

Error message | Description
------------ | ------------
"Ratelimit." | You should consult your subscription and upgrade your package
"Unprocessable Entity" | Check that you are authenticating your `authorization` string correctly

## More about Unprocessable Entity
For illustration purposes, find attached the php class function of `auth()`. This serves as an example of how we build our authorization string.

```php

public function auth()
{
	$b01 = str_replace(['+', '/', '='], ['-', '_', ''], base64_encode('{"typ":"JWT","alg":"HS256"}'));
	$b02 = str_replace(['+', '/', '='], ['-', '_', ''], base64_encode(json_encode($this->payload)));
	$sig = hash_hmac('sha256', $b01 . "." . $b02, $this->api_secret, true);
	$b03 = str_replace(['+', '/', '='], ['-', '_', ''], base64_encode($sig));
	return $b01.'.'.$b02.'.'.$b03;
}

```

## Further help
If you are having issues that you cannot resolve please reach out to us at support@executium.com.


    
