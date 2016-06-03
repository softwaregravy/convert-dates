# convert-dates

[![CircleCI](https://circleci.com/gh/segmentio/convert-dates.svg?style=shield&circle-token=83075c698232f0683037959a50ff604bd3b3d2f0)](https://circleci.com/gh/segmentio/convert-dates)
[![Codecov](https://img.shields.io/codecov/c/github/segmentio/convert-dates/master.svg?maxAge=2592000)](https://codecov.io/gh/segmentio/convert-dates)

Convert all Date instances in an object.

## Installation

```sh
$ npm install @segment/convert-dates
```

## Example

```js
var convert = require('convert-dates');
var obj = { date: new Date() };

obj = convert(obj, function (date) { return 'string'; });

obj.date; // "string"
```

## API

### convertDates(object, converter)
  
Passes all of the `Date` values in an `object` through the `converter` function.
