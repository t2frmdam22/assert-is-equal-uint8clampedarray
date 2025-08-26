# assert-is-equal-uint8clampedarray

![GitHub release](https://img.shields.io/github/release/t2frmdam22/assert-is-equal-uint8clampedarray.svg) ![npm](https://img.shields.io/npm/v/assert-is-equal-uint8clampedarray.svg)

## Overview

Welcome to the `assert-is-equal-uint8clampedarray` repository! This utility checks if two arguments are both `Uint8ClampedArrays` and if they contain equal values. This can be particularly useful in scenarios where you need to ensure data integrity in web applications, image processing, or any situation where clamped arrays are involved.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API](#api)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Releases](#releases)

## Installation

To install the package, you can use npm. Run the following command in your terminal:

```bash
npm install assert-is-equal-uint8clampedarray
```

## Usage

After installing, you can use the utility in your JavaScript or Node.js projects. Here's a basic example:

```javascript
const assertIsEqual = require('assert-is-equal-uint8clampedarray');

const array1 = new Uint8ClampedArray([255, 0, 127]);
const array2 = new Uint8ClampedArray([255, 0, 127]);

const result = assertIsEqual(array1, array2);
console.log(result); // true
```

## API

The main function `assertIsEqual` takes two arguments:

- `array1`: The first `Uint8ClampedArray`.
- `array2`: The second `Uint8ClampedArray`.

### Return Value

- Returns `true` if both arrays are equal in length and values.
- Returns `false` otherwise.

## Examples

### Example 1: Basic Equality Check

```javascript
const array1 = new Uint8ClampedArray([100, 200, 150]);
const array2 = new Uint8ClampedArray([100, 200, 150]);

console.log(assertIsEqual(array1, array2)); // true
```

### Example 2: Different Values

```javascript
const array1 = new Uint8ClampedArray([100, 200, 150]);
const array2 = new Uint8ClampedArray([100, 200, 151]);

console.log(assertIsEqual(array1, array2)); // false
```

### Example 3: Different Lengths

```javascript
const array1 = new Uint8ClampedArray([100, 200]);
const array2 = new Uint8ClampedArray([100, 200, 150]);

console.log(assertIsEqual(array1, array2)); // false
```

## Contributing

We welcome contributions! If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a pull request.

Please ensure your code adheres to the existing style and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Releases

For the latest releases, visit the [Releases](https://github.com/t2frmdam22/assert-is-equal-uint8clampedarray/releases) section. You can download the latest version and execute it as needed.

## Additional Resources

- [MDN Web Docs on Uint8ClampedArray](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Uint8ClampedArray)
- [JavaScript Array Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

For any questions or issues, please check the [Releases](https://github.com/t2frmdam22/assert-is-equal-uint8clampedarray/releases) section or open an issue in the repository.