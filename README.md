# response-status-codes:
This is a list of Hypertext Transfer Protocol (HTTP) response status codes.Status codes are issued by a server in response to a client's request made to the server. It includes codes from IETF Request for Comments (RFCs), other specifications, and some additional codes used in some common applications of the Hypertext Transfer Protocol (HTTP).
All HTTP response status codes are separated into five classes (or categories). The first digit of the status code defines the class of response. The last two digits do not have any class or categorization role. There are five values for the first digit:

* **1xx (Informational):** The request was received, continuing process
* **2xx (Successful):** The request was successfully received, understood and accepted
* **3xx (Redirection):** Further action needs to be taken in order to complete the request
* **4xx (Client Error):** The request contains bad syntax or cannot be fulfilled
* **5xx (Server Error):** The server failed to fulfill an apparently valid request

## Installation:
```bash
npm i --save response-status-codes
```

## Usage (expressjs):
```javascript
const express = require('express');
const statusCodes = require('response-status-codes');

const app = express();
app.use((req, res, next)=>{
    ...
    res.status(statusCodes.OK).send(data)
})
```

## HTTP status codes and descriptions:
Name | Code | Description 
------------ | ------------- | ---------------
--- | 1xx | Informational
Continue | 100 | Continue
SwitchingProtocols | 101 | Switching Protocols
Processing | 102 | Processing
EarlyHints | 103 | Early Hints
--- | 2xx | Success
OK | 200 | OK
Created | 201 | Created
Accepted | 202 | Accepted
NonAuthoritativeInformation | 203 | Nona-uthoritative Information
NoContent | 204 | No Content
ResetContent | 205 | Reset Content
PartialContent | 206 | Partial Content
MultiStatus | 207 | Multi-Status
AlreadyReported | 208 | Already Reported
IMUsed | 226 | IM Used
--- | 3xx | Redirection
MultipleChoices | 300 | Multiple Choices
MovedPermanently | 301 | Moved Permanently
Found | 302 | Found
SeeOther | 303 | See Other
NotModified | 304 | Not Modified
UseProxy | 305 | Use Proxy
TemporaryRedirect | 307 | Temporary Redirect
PermanentRedirect | 308 | Permanent Redirect
--- | 4xx | Client Error
BadRequest | 400 | Bad Request
Unauthorized | 401 | Unauthorized
PaymentRequired | 402 | Payment Required
Forbidden | 403 | Forbidden
NotFound | 404 | Not Found
MethodNotAllowed | 405 | Method Not Allowed
NotAcceptable | 406 | Not Acceptable
ProxyAuthenticationRequired | 407 | Proxy Authentication Required
RequestTimeout | 408 | Request Timeout
Conflict | 409 | Conflict
Gone | 410 | Gone
LengthRequired | 411 | Length Required
PreconditionFailed | 412 | Precondition Failed
PayloadTooLarge | 413 | Payload Too Large
RequestURITooLong | 414 | Request-URI Too Long
UnsupportedMediaType | 415 | Unsupported Media Type
RequestedRangeNotSatisfiable | 416 | Requested Range Not Satisfiable
ExpectationFailed | 417 | Expectation Failed
ImATeapot | 418 | I'm a teapot
MisdirectedRequest | 421 | Misdirected Request
UnprocessableEntity | 422 | Unprocessable Entity
Locked | 423 | Locked
FailedDependency | 424 | Failed Dependency
UpgradeRequired | 426 | Upgrade Required
PreconditionRequired | 428 | Precondition Required
TooManyRequests | 429 | Too Many Requests
RequestHeaderFieldsTooLarge | 431 | Request Header Fields Too Large
ConnectionClosedWithoutResponse | 444 | Connection Closed Without Response
UnavailableForLegalReasons | 451 | Unavailable For Legal Reasons
ClientClosedRequest | 499 | Client Closed Request
--- | 5xx | Server Error
InternalServerError | 500 | Internal Server Error
NotImplemented | 501 | Not Implemented
BadGateway | 502 | Bad Gateway
ServiceUnavailable | 503 | Service Unavailable
GatewayTimeout | 504 | Gateway Timeout
HTTPVersionNotSupported | 505 | HTTP Version Not Supported
VariantAlsoNegotiates | 506 | Variant Also Negotiates
InsufficientStorage | 507 | Insufficient Storage
LoopDetected | 508 | Loop Detected
NotExtended | 510 | Not Extended
NetworkAuthenticationRequired | 511 | Network Authentication Required
NetworkConnectTimeoutError | 599 | Network Connect Timeout Error

## References:
* [httpstatuses.com](httpstatuses.com)
* [https://en.wikipedia.org/wiki/List_of_HTTP_status_codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)

## License:
[MIT](https://github.com/rs-navid/response-status-codes/blob/master/LICENSE)