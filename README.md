# api-documentation for  [boom (v4.3.0)](https://github.com/hapijs/boom#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-boom.svg)](https://travis-ci.org/npmdoc/node-npmdoc-boom)
#### HTTP-friendly error objects

[![NPM](https://nodei.co/npm/boom.png?downloads=true)](https://www.npmjs.com/package/boom)

# html version

- [https://npmdoc.github.io/node-npmdoc-boom/build..beta..travis-ci.org/apidoc.html](https://npmdoc.github.io/node-npmdoc-boom/build..beta..travis-ci.org/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-boom/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-boom_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-boom/build..beta..travis-ci.org/apidoc.html)

# package listing

![package-listing](https://npmdoc.github.io/node-npmdoc-boom/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/hapijs/boom/issues"
    },
    "dependencies": {
        "hoek": "4.x.x"
    },
    "description": "HTTP-friendly error objects",
    "devDependencies": {
        "code": "4.x.x",
        "lab": "13.x.x",
        "markdown-toc": "0.12.x"
    },
    "directories": {},
    "dist": {
        "shasum": "1ed1b4b8cd6891b602910debe33e1d511531b847",
        "tarball": "https://registry.npmjs.org/boom/-/boom-4.3.0.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "gitHead": "cd6790e133b31f1de04430eb50f16ae68714eeae",
    "homepage": "https://github.com/hapijs/boom#readme",
    "keywords": [
        "error",
        "http"
    ],
    "license": "BSD-3-Clause",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "hueniverse",
            "email": "eran@hueniverse.com"
        },
        {
            "name": "wyatt",
            "email": "wpreul@gmail.com"
        },
        {
            "name": "arb",
            "email": "arbretz@gmail.com"
        }
    ],
    "name": "boom",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/hapijs/boom.git"
    },
    "scripts": {
        "test": "lab -a code -t 100 -L -v",
        "test-cov-html": "lab -a code -r html -o coverage.html -L",
        "toc": "node generate-toc.js",
        "version": "npm run toc && git add README.md"
    },
    "version": "4.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module boom](#apidoc.module.boom)
1.  [function <span class="apidocSignatureSpan">boom.</span>badData (message, data)](#apidoc.element.boom.badData)
1.  [function <span class="apidocSignatureSpan">boom.</span>badGateway (message, data)](#apidoc.element.boom.badGateway)
1.  [function <span class="apidocSignatureSpan">boom.</span>badImplementation (message, data)](#apidoc.element.boom.badImplementation)
1.  [function <span class="apidocSignatureSpan">boom.</span>badRequest (message, data)](#apidoc.element.boom.badRequest)
1.  [function <span class="apidocSignatureSpan">boom.</span>clientTimeout (message, data)](#apidoc.element.boom.clientTimeout)
1.  [function <span class="apidocSignatureSpan">boom.</span>conflict (message, data)](#apidoc.element.boom.conflict)
1.  [function <span class="apidocSignatureSpan">boom.</span>create (statusCode, message, data)](#apidoc.element.boom.create)
1.  [function <span class="apidocSignatureSpan">boom.</span>entityTooLarge (message, data)](#apidoc.element.boom.entityTooLarge)
1.  [function <span class="apidocSignatureSpan">boom.</span>expectationFailed (message, data)](#apidoc.element.boom.expectationFailed)
1.  [function <span class="apidocSignatureSpan">boom.</span>forbidden (message, data)](#apidoc.element.boom.forbidden)
1.  [function <span class="apidocSignatureSpan">boom.</span>gatewayTimeout (message, data)](#apidoc.element.boom.gatewayTimeout)
1.  [function <span class="apidocSignatureSpan">boom.</span>illegal (message, data)](#apidoc.element.boom.illegal)
1.  [function <span class="apidocSignatureSpan">boom.</span>internal (message, data, statusCode)](#apidoc.element.boom.internal)
1.  [function <span class="apidocSignatureSpan">boom.</span>lengthRequired (message, data)](#apidoc.element.boom.lengthRequired)
1.  [function <span class="apidocSignatureSpan">boom.</span>locked (message, data)](#apidoc.element.boom.locked)
1.  [function <span class="apidocSignatureSpan">boom.</span>methodNotAllowed (message, data, allow)](#apidoc.element.boom.methodNotAllowed)
1.  [function <span class="apidocSignatureSpan">boom.</span>notAcceptable (message, data)](#apidoc.element.boom.notAcceptable)
1.  [function <span class="apidocSignatureSpan">boom.</span>notFound (message, data)](#apidoc.element.boom.notFound)
1.  [function <span class="apidocSignatureSpan">boom.</span>notImplemented (message, data)](#apidoc.element.boom.notImplemented)
1.  [function <span class="apidocSignatureSpan">boom.</span>paymentRequired (message, data)](#apidoc.element.boom.paymentRequired)
1.  [function <span class="apidocSignatureSpan">boom.</span>preconditionFailed (message, data)](#apidoc.element.boom.preconditionFailed)
1.  [function <span class="apidocSignatureSpan">boom.</span>preconditionRequired (message, data)](#apidoc.element.boom.preconditionRequired)
1.  [function <span class="apidocSignatureSpan">boom.</span>proxyAuthRequired (message, data)](#apidoc.element.boom.proxyAuthRequired)
1.  [function <span class="apidocSignatureSpan">boom.</span>rangeNotSatisfiable (message, data)](#apidoc.element.boom.rangeNotSatisfiable)
1.  [function <span class="apidocSignatureSpan">boom.</span>resourceGone (message, data)](#apidoc.element.boom.resourceGone)
1.  [function <span class="apidocSignatureSpan">boom.</span>serverUnavailable (message, data)](#apidoc.element.boom.serverUnavailable)
1.  [function <span class="apidocSignatureSpan">boom.</span>teapot (message, data)](#apidoc.element.boom.teapot)
1.  [function <span class="apidocSignatureSpan">boom.</span>tooManyRequests (message, data)](#apidoc.element.boom.tooManyRequests)
1.  [function <span class="apidocSignatureSpan">boom.</span>unauthorized (message, scheme, attributes)](#apidoc.element.boom.unauthorized)
1.  [function <span class="apidocSignatureSpan">boom.</span>unsupportedMediaType (message, data)](#apidoc.element.boom.unsupportedMediaType)
1.  [function <span class="apidocSignatureSpan">boom.</span>uriTooLong (message, data)](#apidoc.element.boom.uriTooLong)
1.  [function <span class="apidocSignatureSpan">boom.</span>wrap (error, statusCode, message)](#apidoc.element.boom.wrap)



# <a name="apidoc.module.boom"></a>[module boom](#apidoc.module.boom)

#### <a name="apidoc.element.boom.badData"></a>[function <span class="apidocSignatureSpan">boom.</span>badData (message, data)](#apidoc.element.boom.badData)
- description and source-code
```javascript
badData = function (message, data) {

    return internals.create(422, message, data, exports.badData);
}
```
- example usage
```shell
...
  - ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
  - ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
  - ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
  - ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
  - ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
  - ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
  - ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
  - ['Boom.badData([message], [data])'](#boombaddatamessage-data)
  - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
  - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
  - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
  - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
- [HTTP 5xx Errors](#http-5xx-errors)
  - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
  - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
...
```

#### <a name="apidoc.element.boom.badGateway"></a>[function <span class="apidocSignatureSpan">boom.</span>badGateway (message, data)](#apidoc.element.boom.badGateway)
- description and source-code
```javascript
badGateway = function (message, data) {

    return internals.serverError(message, data, 502, exports.badGateway);
}
```
- example usage
```shell
...
    - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
    - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
    - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
    - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
  - [HTTP 5xx Errors](#http-5xx-errors)
    - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
    - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
    - ['Boom.badGateway([message], [data])'](#boombadgatewaymessage-data)
    - ['Boom.serverUnavailable([message], [data])'](#boomserverunavailablemessage-data)
    - ['Boom.gatewayTimeout([message], [data])'](#boomgatewaytimeoutmessage-data)
  - [F.A.Q.](#faq)

<!-- tocstop -->

# Boom
...
```

#### <a name="apidoc.element.boom.badImplementation"></a>[function <span class="apidocSignatureSpan">boom.</span>badImplementation (message, data)](#apidoc.element.boom.badImplementation)
- description and source-code
```javascript
badImplementation = function (message, data) {

    const err = internals.serverError(message, data, 500, exports.badImplementation);
    err.isDeveloperError = true;
    return err;
}
```
- example usage
```shell
...
    - ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
    - ['Boom.badData([message], [data])'](#boombaddatamessage-data)
    - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
    - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
    - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
    - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
  - [HTTP 5xx Errors](#http-5xx-errors)
    - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
    - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
    - ['Boom.badGateway([message], [data])'](#boombadgatewaymessage-data)
    - ['Boom.serverUnavailable([message], [data])'](#boomserverunavailablemessage-data)
    - ['Boom.gatewayTimeout([message], [data])'](#boomgatewaytimeoutmessage-data)
  - [F.A.Q.](#faq)

<!-- tocstop -->
...
```

#### <a name="apidoc.element.boom.badRequest"></a>[function <span class="apidocSignatureSpan">boom.</span>badRequest (message, data)](#apidoc.element.boom.badRequest)
- description and source-code
```javascript
badRequest = function (message, data) {

    return internals.create(400, message, data, exports.badRequest);
}
```
- example usage
```shell
...
<!-- toc -->

- [Boom](#boom)
- [Helper Methods](#helper-methods)
  - ['wrap(error, [statusCode], [message])'](#wraperror-statuscode-message)
  - ['create(statusCode, [message], [data])'](#createstatuscode-message-data)
- [HTTP 4xx Errors](#http-4xx-errors)
  - ['Boom.badRequest([message], [data])'](#boombadrequestmessage-data)
  - ['Boom.unauthorized([message], [scheme], [attributes])'](#boomunauthorizedmessage-scheme-attributes)
  - ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
  - ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
  - ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
  - ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
  - ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
  - ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
...
```

#### <a name="apidoc.element.boom.clientTimeout"></a>[function <span class="apidocSignatureSpan">boom.</span>clientTimeout (message, data)](#apidoc.element.boom.clientTimeout)
- description and source-code
```javascript
clientTimeout = function (message, data) {

    return internals.create(408, message, data, exports.clientTimeout);
}
```
- example usage
```shell
...
- ['Boom.unauthorized([message], [scheme], [attributes])'](#boomunauthorizedmessage-scheme-attributes)
- ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
- ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
- ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
- ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
- ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
- ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
- ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
...
```

#### <a name="apidoc.element.boom.conflict"></a>[function <span class="apidocSignatureSpan">boom.</span>conflict (message, data)](#apidoc.element.boom.conflict)
- description and source-code
```javascript
conflict = function (message, data) {

    return internals.create(409, message, data, exports.conflict);
}
```
- example usage
```shell
...
- ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
- ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
- ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
- ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
- ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
- ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
- ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
- ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
...
```

#### <a name="apidoc.element.boom.create"></a>[function <span class="apidocSignatureSpan">boom.</span>create (statusCode, message, data)](#apidoc.element.boom.create)
- description and source-code
```javascript
create = function (statusCode, message, data) {

    return internals.create(statusCode, message, data, exports.create);
}
```
- example usage
```shell
...

Generates an 'Error' object with the **boom** decorations where:
- 'statusCode' - an HTTP error code number. Must be greater or equal 400.
- 'message' - optional message string.
- 'data' - additional error data set to 'error.data' property.

'''js
var error = Boom.create(400, 'Bad request', { timestamp: Date.now() });
'''

## HTTP 4xx Errors

### 'Boom.badRequest([message], [data])'

Returns a 400 Bad Request error where:
...
```

#### <a name="apidoc.element.boom.entityTooLarge"></a>[function <span class="apidocSignatureSpan">boom.</span>entityTooLarge (message, data)](#apidoc.element.boom.entityTooLarge)
- description and source-code
```javascript
entityTooLarge = function (message, data) {

    return internals.create(413, message, data, exports.entityTooLarge);
}
```
- example usage
```shell
...
- ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
- ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
- ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
- ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
- ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
- ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
- ['Boom.badData([message], [data])'](#boombaddatamessage-data)
- ['Boom.locked([message], [data])'](#boomlockedmessage-data)
...
```

#### <a name="apidoc.element.boom.expectationFailed"></a>[function <span class="apidocSignatureSpan">boom.</span>expectationFailed (message, data)](#apidoc.element.boom.expectationFailed)
- description and source-code
```javascript
expectationFailed = function (message, data) {

    return internals.create(417, message, data, exports.expectationFailed);
}
```
- example usage
```shell
...
  - ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
  - ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
  - ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
  - ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
  - ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
  - ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
  - ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
  - ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
  - ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
  - ['Boom.badData([message], [data])'](#boombaddatamessage-data)
  - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
  - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
  - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
  - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
- [HTTP 5xx Errors](#http-5xx-errors)
...
```

#### <a name="apidoc.element.boom.forbidden"></a>[function <span class="apidocSignatureSpan">boom.</span>forbidden (message, data)](#apidoc.element.boom.forbidden)
- description and source-code
```javascript
forbidden = function (message, data) {

    return internals.create(403, message, data, exports.forbidden);
}
```
- example usage
```shell
...
- [Helper Methods](#helper-methods)
  - ['wrap(error, [statusCode], [message])'](#wraperror-statuscode-message)
  - ['create(statusCode, [message], [data])'](#createstatuscode-message-data)
- [HTTP 4xx Errors](#http-4xx-errors)
  - ['Boom.badRequest([message], [data])'](#boombadrequestmessage-data)
  - ['Boom.unauthorized([message], [scheme], [attributes])'](#boomunauthorizedmessage-scheme-attributes)
  - ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
  - ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
  - ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
  - ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
  - ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
  - ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
  - ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
  - ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
  - ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
...
```

#### <a name="apidoc.element.boom.gatewayTimeout"></a>[function <span class="apidocSignatureSpan">boom.</span>gatewayTimeout (message, data)](#apidoc.element.boom.gatewayTimeout)
- description and source-code
```javascript
gatewayTimeout = function (message, data) {

    return internals.serverError(message, data, 504, exports.gatewayTimeout);
}
```
- example usage
```shell
...
    - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
    - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
  - [HTTP 5xx Errors](#http-5xx-errors)
    - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
    - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
    - ['Boom.badGateway([message], [data])'](#boombadgatewaymessage-data)
    - ['Boom.serverUnavailable([message], [data])'](#boomserverunavailablemessage-data)
    - ['Boom.gatewayTimeout([message], [data])'](#boomgatewaytimeoutmessage-data)
  - [F.A.Q.](#faq)

<!-- tocstop -->

# Boom

**boom** provides a set of utilities for returning HTTP errors. Each utility returns a 'Boom' error response
...
```

#### <a name="apidoc.element.boom.illegal"></a>[function <span class="apidocSignatureSpan">boom.</span>illegal (message, data)](#apidoc.element.boom.illegal)
- description and source-code
```javascript
illegal = function (message, data) {

    return internals.create(451, message, data, exports.illegal);
}
```
- example usage
```shell
...
  - ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
  - ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
  - ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
  - ['Boom.badData([message], [data])'](#boombaddatamessage-data)
  - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
  - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
  - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
  - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
- [HTTP 5xx Errors](#http-5xx-errors)
  - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
  - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
  - ['Boom.badGateway([message], [data])'](#boombadgatewaymessage-data)
  - ['Boom.serverUnavailable([message], [data])'](#boomserverunavailablemessage-data)
  - ['Boom.gatewayTimeout([message], [data])'](#boomgatewaytimeoutmessage-data)
- [F.A.Q.](#faq)
...
```

#### <a name="apidoc.element.boom.internal"></a>[function <span class="apidocSignatureSpan">boom.</span>internal (message, data, statusCode)](#apidoc.element.boom.internal)
- description and source-code
```javascript
internal = function (message, data, statusCode) {

    return internals.serverError(message, data, statusCode, exports.internal);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.boom.lengthRequired"></a>[function <span class="apidocSignatureSpan">boom.</span>lengthRequired (message, data)](#apidoc.element.boom.lengthRequired)
- description and source-code
```javascript
lengthRequired = function (message, data) {

    return internals.create(411, message, data, exports.lengthRequired);
}
```
- example usage
```shell
...
- ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
- ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
- ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
- ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
- ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
- ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
- ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
- ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
...
```

#### <a name="apidoc.element.boom.locked"></a>[function <span class="apidocSignatureSpan">boom.</span>locked (message, data)](#apidoc.element.boom.locked)
- description and source-code
```javascript
locked = function (message, data) {

    return internals.create(423, message, data, exports.locked);
}
```
- example usage
```shell
...
  - ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
  - ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
  - ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
  - ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
  - ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
  - ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
  - ['Boom.badData([message], [data])'](#boombaddatamessage-data)
  - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
  - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
  - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
  - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
- [HTTP 5xx Errors](#http-5xx-errors)
  - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
  - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
  - ['Boom.badGateway([message], [data])'](#boombadgatewaymessage-data)
...
```

#### <a name="apidoc.element.boom.methodNotAllowed"></a>[function <span class="apidocSignatureSpan">boom.</span>methodNotAllowed (message, data, allow)](#apidoc.element.boom.methodNotAllowed)
- description and source-code
```javascript
methodNotAllowed = function (message, data, allow) {

    const err = internals.create(405, message, data, exports.methodNotAllowed);

    if (typeof allow === 'string') {
        allow = [allow];
    }

    if (Array.isArray(allow)) {
        err.output.headers.Allow = allow.join(', ');
    }

    return err;
}
```
- example usage
```shell
...
  - ['create(statusCode, [message], [data])'](#createstatuscode-message-data)
- [HTTP 4xx Errors](#http-4xx-errors)
  - ['Boom.badRequest([message], [data])'](#boombadrequestmessage-data)
  - ['Boom.unauthorized([message], [scheme], [attributes])'](#boomunauthorizedmessage-scheme-attributes)
  - ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
  - ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
  - ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
  - ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
  - ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
  - ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
  - ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
  - ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
  - ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
  - ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
  - ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
...
```

#### <a name="apidoc.element.boom.notAcceptable"></a>[function <span class="apidocSignatureSpan">boom.</span>notAcceptable (message, data)](#apidoc.element.boom.notAcceptable)
- description and source-code
```javascript
notAcceptable = function (message, data) {

    return internals.create(406, message, data, exports.notAcceptable);
}
```
- example usage
```shell
...
  - [HTTP 4xx Errors](#http-4xx-errors)
- ['Boom.badRequest([message], [data])'](#boombadrequestmessage-data)
- ['Boom.unauthorized([message], [scheme], [attributes])'](#boomunauthorizedmessage-scheme-attributes)
- ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
- ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
- ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
- ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
- ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
- ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
...
```

#### <a name="apidoc.element.boom.notFound"></a>[function <span class="apidocSignatureSpan">boom.</span>notFound (message, data)](#apidoc.element.boom.notFound)
- description and source-code
```javascript
notFound = function (message, data) {

    return internals.create(404, message, data, exports.notFound);
}
```
- example usage
```shell
...
  - ['wrap(error, [statusCode], [message])'](#wraperror-statuscode-message)
  - ['create(statusCode, [message], [data])'](#createstatuscode-message-data)
- [HTTP 4xx Errors](#http-4xx-errors)
  - ['Boom.badRequest([message], [data])'](#boombadrequestmessage-data)
  - ['Boom.unauthorized([message], [scheme], [attributes])'](#boomunauthorizedmessage-scheme-attributes)
  - ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
  - ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
  - ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
  - ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
  - ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
  - ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
  - ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
  - ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
  - ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
  - ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
...
```

#### <a name="apidoc.element.boom.notImplemented"></a>[function <span class="apidocSignatureSpan">boom.</span>notImplemented (message, data)](#apidoc.element.boom.notImplemented)
- description and source-code
```javascript
notImplemented = function (message, data) {

    return internals.serverError(message, data, 501, exports.notImplemented);
}
```
- example usage
```shell
...
    - ['Boom.badData([message], [data])'](#boombaddatamessage-data)
    - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
    - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
    - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
    - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
  - [HTTP 5xx Errors](#http-5xx-errors)
    - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
    - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
    - ['Boom.badGateway([message], [data])'](#boombadgatewaymessage-data)
    - ['Boom.serverUnavailable([message], [data])'](#boomserverunavailablemessage-data)
    - ['Boom.gatewayTimeout([message], [data])'](#boomgatewaytimeoutmessage-data)
  - [F.A.Q.](#faq)

<!-- tocstop -->
...
```

#### <a name="apidoc.element.boom.paymentRequired"></a>[function <span class="apidocSignatureSpan">boom.</span>paymentRequired (message, data)](#apidoc.element.boom.paymentRequired)
- description and source-code
```javascript
paymentRequired = function (message, data) {

    return internals.create(402, message, data, exports.paymentRequired);
}
```
- example usage
```shell
...
- [Boom](#boom)
- [Helper Methods](#helper-methods)
  - ['wrap(error, [statusCode], [message])'](#wraperror-statuscode-message)
  - ['create(statusCode, [message], [data])'](#createstatuscode-message-data)
- [HTTP 4xx Errors](#http-4xx-errors)
  - ['Boom.badRequest([message], [data])'](#boombadrequestmessage-data)
  - ['Boom.unauthorized([message], [scheme], [attributes])'](#boomunauthorizedmessage-scheme-attributes)
  - ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
  - ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
  - ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
  - ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
  - ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
  - ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
  - ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
  - ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
...
```

#### <a name="apidoc.element.boom.preconditionFailed"></a>[function <span class="apidocSignatureSpan">boom.</span>preconditionFailed (message, data)](#apidoc.element.boom.preconditionFailed)
- description and source-code
```javascript
preconditionFailed = function (message, data) {

    return internals.create(412, message, data, exports.preconditionFailed);
}
```
- example usage
```shell
...
- ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
- ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
- ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
- ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
- ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
- ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
- ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
- ['Boom.badData([message], [data])'](#boombaddatamessage-data)
...
```

#### <a name="apidoc.element.boom.preconditionRequired"></a>[function <span class="apidocSignatureSpan">boom.</span>preconditionRequired (message, data)](#apidoc.element.boom.preconditionRequired)
- description and source-code
```javascript
preconditionRequired = function (message, data) {

    return internals.create(428, message, data, exports.preconditionRequired);
}
```
- example usage
```shell
...
  - ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
  - ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
  - ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
  - ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
  - ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
  - ['Boom.badData([message], [data])'](#boombaddatamessage-data)
  - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
  - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
  - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
  - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
- [HTTP 5xx Errors](#http-5xx-errors)
  - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
  - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
  - ['Boom.badGateway([message], [data])'](#boombadgatewaymessage-data)
  - ['Boom.serverUnavailable([message], [data])'](#boomserverunavailablemessage-data)
...
```

#### <a name="apidoc.element.boom.proxyAuthRequired"></a>[function <span class="apidocSignatureSpan">boom.</span>proxyAuthRequired (message, data)](#apidoc.element.boom.proxyAuthRequired)
- description and source-code
```javascript
proxyAuthRequired = function (message, data) {

    return internals.create(407, message, data, exports.proxyAuthRequired);
}
```
- example usage
```shell
...
- ['Boom.badRequest([message], [data])'](#boombadrequestmessage-data)
- ['Boom.unauthorized([message], [scheme], [attributes])'](#boomunauthorizedmessage-scheme-attributes)
- ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
- ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
- ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
- ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
- ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
- ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
...
```

#### <a name="apidoc.element.boom.rangeNotSatisfiable"></a>[function <span class="apidocSignatureSpan">boom.</span>rangeNotSatisfiable (message, data)](#apidoc.element.boom.rangeNotSatisfiable)
- description and source-code
```javascript
rangeNotSatisfiable = function (message, data) {

    return internals.create(416, message, data, exports.rangeNotSatisfiable);
}
```
- example usage
```shell
...
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
- ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
- ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
- ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
- ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
- ['Boom.badData([message], [data])'](#boombaddatamessage-data)
- ['Boom.locked([message], [data])'](#boomlockedmessage-data)
- ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
- ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
- ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
...
```

#### <a name="apidoc.element.boom.resourceGone"></a>[function <span class="apidocSignatureSpan">boom.</span>resourceGone (message, data)](#apidoc.element.boom.resourceGone)
- description and source-code
```javascript
resourceGone = function (message, data) {

    return internals.create(410, message, data, exports.resourceGone);
}
```
- example usage
```shell
...
- ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
- ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
- ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
- ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
- ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
- ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
- ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
- ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
...
```

#### <a name="apidoc.element.boom.serverUnavailable"></a>[function <span class="apidocSignatureSpan">boom.</span>serverUnavailable (message, data)](#apidoc.element.boom.serverUnavailable)
- description and source-code
```javascript
serverUnavailable = function (message, data) {

    return internals.serverError(message, data, 503, exports.serverUnavailable);
}
```
- example usage
```shell
...
    - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
    - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
    - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
  - [HTTP 5xx Errors](#http-5xx-errors)
    - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
    - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
    - ['Boom.badGateway([message], [data])'](#boombadgatewaymessage-data)
    - ['Boom.serverUnavailable([message], [data])'](#boomserverunavailablemessage-data)
    - ['Boom.gatewayTimeout([message], [data])'](#boomgatewaytimeoutmessage-data)
  - [F.A.Q.](#faq)

<!-- tocstop -->

# Boom
...
```

#### <a name="apidoc.element.boom.teapot"></a>[function <span class="apidocSignatureSpan">boom.</span>teapot (message, data)](#apidoc.element.boom.teapot)
- description and source-code
```javascript
teapot = function (message, data) {

    return internals.create(418, message, data, exports.teapot);
}
```
- example usage
```shell
...
  - ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
  - ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
  - ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
  - ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
  - ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
  - ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
  - ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
  - ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
  - ['Boom.badData([message], [data])'](#boombaddatamessage-data)
  - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
  - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
  - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
  - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
- [HTTP 5xx Errors](#http-5xx-errors)
  - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
...
```

#### <a name="apidoc.element.boom.tooManyRequests"></a>[function <span class="apidocSignatureSpan">boom.</span>tooManyRequests (message, data)](#apidoc.element.boom.tooManyRequests)
- description and source-code
```javascript
tooManyRequests = function (message, data) {

    return internals.create(429, message, data, exports.tooManyRequests);
}
```
- example usage
```shell
...
  - ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
  - ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
  - ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
  - ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
  - ['Boom.badData([message], [data])'](#boombaddatamessage-data)
  - ['Boom.locked([message], [data])'](#boomlockedmessage-data)
  - ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
  - ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
  - ['Boom.illegal([message], [data])'](#boomillegalmessage-data)
- [HTTP 5xx Errors](#http-5xx-errors)
  - ['Boom.badImplementation([message], [data])' - (*alias: 'internal'*)](#boombadimplementationmessage-data---alias-internal)
  - ['Boom.notImplemented([message], [data])'](#boomnotimplementedmessage-data)
  - ['Boom.badGateway([message], [data])'](#boombadgatewaymessage-data)
  - ['Boom.serverUnavailable([message], [data])'](#boomserverunavailablemessage-data)
  - ['Boom.gatewayTimeout([message], [data])'](#boomgatewaytimeoutmessage-data)
...
```

#### <a name="apidoc.element.boom.unauthorized"></a>[function <span class="apidocSignatureSpan">boom.</span>unauthorized (message, scheme, attributes)](#apidoc.element.boom.unauthorized)
- description and source-code
```javascript
unauthorized = function (message, scheme, attributes) {          // Or function (message, wwwAuthenticate[])

    const err = internals.create(401, message, undefined, exports.unauthorized);

    if (!scheme) {
        return err;
    }

    let wwwAuthenticate = '';

    if (typeof scheme === 'string') {

        // function (message, scheme, attributes)

        wwwAuthenticate = scheme;

        if (attributes || message) {
            err.output.payload.attributes = {};
        }

        if (attributes) {
            if (typeof attributes === 'string') {
                wwwAuthenticate = wwwAuthenticate + ' ' + Hoek.escapeHeaderAttribute(attributes);
                err.output.payload.attributes = attributes;
            }
            else {
                const names = Object.keys(attributes);
                for (let i = 0; i < names.length; ++i) {
                    const name = names[i];
                    if (i) {
                        wwwAuthenticate = wwwAuthenticate + ',';
                    }

                    let value = attributes[name];
                    if (value === null ||
                        value === undefined) {              // Value can be zero

                        value = '';
                    }
                    wwwAuthenticate = wwwAuthenticate + ' ' + name + '="' + Hoek.escapeHeaderAttribute(value.toString()) + '"';
                    err.output.payload.attributes[name] = value;
                }
            }
        }


        if (message) {
            if (attributes) {
                wwwAuthenticate = wwwAuthenticate + ',';
            }
            wwwAuthenticate = wwwAuthenticate + ' error="' + Hoek.escapeHeaderAttribute(message) + '"';
            err.output.payload.attributes.error = message;
        }
        else {
            err.isMissing = true;
        }
    }
    else {

        // function (message, wwwAuthenticate[])

        const wwwArray = scheme;
        for (let i = 0; i < wwwArray.length; ++i) {
            if (i) {
                wwwAuthenticate = wwwAuthenticate + ', ';
            }

            wwwAuthenticate = wwwAuthenticate + wwwArray[i];
        }
    }

    err.output.headers['WWW-Authenticate'] = wwwAuthenticate;

    return err;
}
```
- example usage
```shell
...

- [Boom](#boom)
- [Helper Methods](#helper-methods)
  - ['wrap(error, [statusCode], [message])'](#wraperror-statuscode-message)
  - ['create(statusCode, [message], [data])'](#createstatuscode-message-data)
- [HTTP 4xx Errors](#http-4xx-errors)
  - ['Boom.badRequest([message], [data])'](#boombadrequestmessage-data)
  - ['Boom.unauthorized([message], [scheme], [attributes])'](#boomunauthorizedmessage-scheme-attributes)
  - ['Boom.paymentRequired([message], [data])'](#boompaymentrequiredmessage-data)
  - ['Boom.forbidden([message], [data])'](#boomforbiddenmessage-data)
  - ['Boom.notFound([message], [data])'](#boomnotfoundmessage-data)
  - ['Boom.methodNotAllowed([message], [data], [allow])'](#boommethodnotallowedmessage-data-allow)
  - ['Boom.notAcceptable([message], [data])'](#boomnotacceptablemessage-data)
  - ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
  - ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
...
```

#### <a name="apidoc.element.boom.unsupportedMediaType"></a>[function <span class="apidocSignatureSpan">boom.</span>unsupportedMediaType (message, data)](#apidoc.element.boom.unsupportedMediaType)
- description and source-code
```javascript
unsupportedMediaType = function (message, data) {

    return internals.create(415, message, data, exports.unsupportedMediaType);
}
```
- example usage
```shell
...
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
- ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
- ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
- ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
- ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
- ['Boom.badData([message], [data])'](#boombaddatamessage-data)
- ['Boom.locked([message], [data])'](#boomlockedmessage-data)
- ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
- ['Boom.tooManyRequests([message], [data])'](#boomtoomanyrequestsmessage-data)
...
```

#### <a name="apidoc.element.boom.uriTooLong"></a>[function <span class="apidocSignatureSpan">boom.</span>uriTooLong (message, data)](#apidoc.element.boom.uriTooLong)
- description and source-code
```javascript
uriTooLong = function (message, data) {

    return internals.create(414, message, data, exports.uriTooLong);
}
```
- example usage
```shell
...
- ['Boom.proxyAuthRequired([message], [data])'](#boomproxyauthrequiredmessage-data)
- ['Boom.clientTimeout([message], [data])'](#boomclienttimeoutmessage-data)
- ['Boom.conflict([message], [data])'](#boomconflictmessage-data)
- ['Boom.resourceGone([message], [data])'](#boomresourcegonemessage-data)
- ['Boom.lengthRequired([message], [data])'](#boomlengthrequiredmessage-data)
- ['Boom.preconditionFailed([message], [data])'](#boompreconditionfailedmessage-data)
- ['Boom.entityTooLarge([message], [data])'](#boomentitytoolargemessage-data)
- ['Boom.uriTooLong([message], [data])'](#boomuritoolongmessage-data)
- ['Boom.unsupportedMediaType([message], [data])'](#boomunsupportedmediatypemessage-data)
- ['Boom.rangeNotSatisfiable([message], [data])'](#boomrangenotsatisfiablemessage-data)
- ['Boom.expectationFailed([message], [data])'](#boomexpectationfailedmessage-data)
- ['Boom.teapot([message], [data])'](#boomteapotmessage-data)
- ['Boom.badData([message], [data])'](#boombaddatamessage-data)
- ['Boom.locked([message], [data])'](#boomlockedmessage-data)
- ['Boom.preconditionRequired([message], [data])'](#boompreconditionrequiredmessage-data)
...
```

#### <a name="apidoc.element.boom.wrap"></a>[function <span class="apidocSignatureSpan">boom.</span>wrap (error, statusCode, message)](#apidoc.element.boom.wrap)
- description and source-code
```javascript
wrap = function (error, statusCode, message) {

    Hoek.assert(error instanceof Error, 'Cannot wrap non-Error object');
    Hoek.assert(!error.isBoom || arguments.length === 1, 'Cannot provide statusCode or message with boom error');

    return (error.isBoom ? error : internals.initialize(error, statusCode || 500, message));
}
```
- example usage
```shell
...
- 'error' - the error object to wrap. If 'error' is already a **boom** object, returns back the same object.
- 'statusCode' - optional HTTP status code. Defaults to '500'.
- 'message' - optional message string. If the error already has a message, it adds the message as a prefix.
  Defaults to no message.

'''js
var error = new Error('Unexpected input');
Boom.wrap(error, 400);
'''

### 'create(statusCode, [message], [data])'

Generates an 'Error' object with the **boom** decorations where:
- 'statusCode' - an HTTP error code number. Must be greater or equal 400.
- 'message' - optional message string.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
