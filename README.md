# mis-configurator

[![NPM version](https://img.shields.io/npm/v/mis-configurator.svg?style=flat-square)](https://npmjs.org/package/mis-configurator)

> A node module to decode/encode a Miscreated hosting.cfg file.

## Install

    $ npm install --save mis-configurator

## Usage

```js
import {
	createHostingCFGStringFromObject,
	createObjectFromHostingCFGString
} from 'mis-configurator';

const hostingCFGString = createHostingCFGStringFromObject(mockHostingCFGObj);
const hostingCFGObj = createObjectFromHostingCFGString(mockHostingCFgString);
```

## API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

-   [saneDefaults](#sanedefaults)
-   [MisConfigurator](#misconfigurator)
    -   [decode](#decode)
    -   [encode](#encode)
    -   [detectLineEnding](#detectlineending)
    -   [stringBeginsWithOnOfTheseStrings](#stringbeginswithonofthesestrings)
-   [createHostingCFGStringFromObject](#createhostingcfgstringfromobject)
-   [createObjectFromHostingCFGString](#createobjectfromhostingcfgstring)

### saneDefaults

MisConfigurator
project: mis-configurator
author: Chris Sprance - csprance

### MisConfigurator

Encode and decode Miscreated hosting.cfg files
decode to get a simple js object / encode to get a config-String

**Parameters**

-   `options` **MisConfiguratorOptions**  (optional, default `defaultOptions`)

**Meta**

-   **author**: Csprance - Based off of config-cfg-ini

#### decode

Decode a config-string

**Parameters**

-   `data` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** {string}

Returns **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** object

#### encode

Encode an object
no nesting section supported!

**Parameters**

-   `object` **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** {object}

Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** 

#### detectLineEnding

Try to detect the used line ending
(windows, unix, mac)

**Parameters**

-   `data` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** 

Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** string

#### stringBeginsWithOnOfTheseStrings

Figures out if a string begins with one of the string
(windows, unix, mac)

**Parameters**

-   `string` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** 
-   `stringList` **[Array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array)&lt;[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)>** 

Returns **[boolean](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** string

### createHostingCFGStringFromObject

This takes a javascript object and transforms it to a hosting.cfg string.

**Parameters**

-   `data` **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** The javascript object to transform.

Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** a hosting.cfg string.

### createObjectFromHostingCFGString

This takes a hosting.cfg string and transforms it to a javascript object

**Parameters**

-   `str` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The string hosting.cfg to transform.

Returns **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** a javascript object

## License

MIT © [csprance](https://github.com/csprance)
