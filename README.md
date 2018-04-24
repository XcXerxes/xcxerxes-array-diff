# xcxerxes-array-diff [![npm](https://img.shields.io/npm/v/xcxerxes-array-diff.svg)](https://www.npmjs.com/package/xcxerxes-array-diff) [![Build Status](https://travis-ci.org/XcXerxes/xcxerxes-array-diff.svg)](https://travis-ci.org/XcXerxes/xcxerxes-array-diff.svg)

Returns an array with only the unique values present in all given arrays using strict equality for comparisons.

## Example

```javascript

const diff = require('xcxerxes-array-diff')

console.log(diff([1, 2, 3], [2, 3]))
// -> [1]

console.log(diff([1, 2, 3, 4, 4, 4], [1, 2]))
// -> [3, 4, 4, 4]

console.log(diff([1, 2, 3, 4, 5], [2, 3], [4]))
// -> [1, 5]

console.log(diff([1, 2, 3], [1, 2, 3]))
// -> []

console.log(diff([1, 2, 3], []))
// -> [1, 2, 3]

console.log(diff([1, 2, 3], null))
// -> [1, 2, 3]
```

## License
Copyright © 2018 [xcxerxes](https://github.com/XcXerxes)
Released under the MIT license
