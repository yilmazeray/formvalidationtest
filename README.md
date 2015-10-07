# validate.js [![Build Status](https://travis-ci.org/dleitee/valid.js.svg?branch=master)](https://travis-ci.org/dleitee/valid.js)
A simple library for data validation.

## Install

**Unavailable temporarily**

ValidateJS is available on npm:
```
npm install validatejs --save
```

or bower:
```
bower install validatejs
```

## Usage

### With ES6/import

```javascript
import {validate, string, util} from 'validate'

let isvalid = validate(string.maxLength(15), util.required)
let result = isvalid('Test ValidateJS')
// result => true
```

### With require

```javascript
var validatejs = require('validate')
var validate = validatejs.validate,
    string = validatejs.string,
    util = validatejs.util

var isvalid = validate(string.maxLength(15), util.required)
var result = isvalid('Test ValidateJS')
// result => true
```

### With Browser

```html
<script src="validate.js/validate.min.js"></script>
```

```javascript
var validate = validate.validate
var string = validate.string
var util = validate.util

var isvalid = validate(string.maxLength(15), util.required)
var result = isvalid('Test ValidateJS')
// result => true
```
OR
```javascript
var validate = window.validate.validate
var string = window.validate.string
var util = window.validate.util

var isvalid = validate(string.maxLength(15), util.required)
var result = isvalid('Test ValidateJS')
// result => true
```

Also available for [AMD](https://github.com/amdjs/amdjs-api/wiki/AMD)

# Validation Functions

- [x] [String](https://github.com/dleitee/valid.js/blob/master/docs/string.md)
    - [x] isString
    - [x] minLength(min)
    - [x] maxLength(max)
    - [x] length(min, max)
    - [x] regex(reg)
- [x] [Number](https://github.com/dleitee/valid.js/blob/master/docs/number.md)
    - [x] isNumber
    - [x] minNumber
    - [x] maxNumber
    - [x] between
-  [x] [Util](https://github.com/dleitee/valid.js/blob/master/docs/util.md)
    - [x] isRequired
    - [x] isEmail

# LICENSE
The MIT License (MIT)

Copyright (c) 2015 Daniel Leite de Oliveira

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

