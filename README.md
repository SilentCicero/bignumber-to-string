# bignumber-to-string

```
npm install bignumber-to-string
```

A tiny module to convert nested objects or arrays containing BigNumbers to strings

## Example

```js
const bigNumberToString = require('bignumber-to-string')

const obj = {
  data: 100,
  somedata: 'sdfsdfsd',
  bn: new BigNumber(1000),
  something: {
    bn: new BigNumber(10000)
  }
}

console.log(bigNumberToString(obj))
/*
returns:
{
  data: 100,
  somedata: 'sdfsdfsd',
  bn: '1000',
  something: {
    bn: '10000'
  }
}
*/
```

## Tests

```
npm test
```

## License

```
The MIT License (MIT)

Copyright (c) 2016 Nick Dodson

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```