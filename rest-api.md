**Table of Contents**

  - [Accessibility](#accessibility)
  - [General Information](#general-information)
  - [HTTP Return Codes](#http-return-codes)
  - [Error Codes](#error-codes)
  - [General Information on Endpoints](#general-information-on-endpoints)
  
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
* HTTP `429` return code is used when breaking a request rate limit.
* HTTP `418` return code is used when an IP has been banned automatically for continuing to send requests after receiving `429` codes.
* HTTP `5XX` return codes are used for internal errors where the issue is with the executium side.

