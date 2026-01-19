# Array Base Assert Any Has Property

![GitHub Release](https://img.shields.io/github/v/release/ShalkyFidelis/array-base-assert-any-has-property?color=blue&label=Latest%20Release)

## Overview

Welcome to the **Array Base Assert Any Has Property** repository! This project provides a simple and effective way to check if at least one element in a given array possesses a specified property. This property can be either an own property or an inherited one. The utility is designed to be lightweight and easy to use in any JavaScript environment, including Node.js.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Reference](#api-reference)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Features

- **Simple Interface**: Easy to use with minimal setup.
- **Flexible Checks**: Works with both own and inherited properties.
- **Lightweight**: Minimal impact on performance.
- **Compatibility**: Works seamlessly with Node.js and browsers.

## Installation

To get started, you need to install the package. You can do this using npm or yarn. Run one of the following commands in your terminal:

```bash
npm install array-base-assert-any-has-property
```

or

```bash
yarn add array-base-assert-any-has-property
```

## Usage

After installing the package, you can use it in your project. Here’s a simple example of how to get started:

```javascript
const hasProperty = require('array-base-assert-any-has-property');

const array = [{ name: 'Alice' }, { age: 30 }, { job: 'Engineer' }];

const result = hasProperty(array, 'age');
console.log(result); // true
```

## API Reference

### `hasProperty(array, property)`

- **Parameters**:
  - `array`: An array of objects to be checked.
  - `property`: A string representing the property name to check for.

- **Returns**: 
  - `true` if at least one object in the array has the specified property.
  - `false` otherwise.

### Example

```javascript
const array = [{ name: 'Alice' }, { age: 30 }, { job: 'Engineer' }];
console.log(hasProperty(array, 'name')); // true
console.log(hasProperty(array, 'salary')); // false
```

## Examples

Here are a few more examples to illustrate how the utility works:

### Example 1: Checking Own Properties

```javascript
const array = [{ name: 'Alice' }, { age: 30 }, { job: 'Engineer' }];
console.log(hasProperty(array, 'job')); // true
```

### Example 2: Checking Inherited Properties

```javascript
function Person(name, age) {
  this.name = name;
  this.age = age;
}

const array = [new Person('Alice', 30), new Person('Bob', 25)];
console.log(hasProperty(array, 'age')); // true
```

### Example 3: No Matching Property

```javascript
const array = [{ name: 'Alice' }, { job: 'Engineer' }];
console.log(hasProperty(array, 'salary')); // false
```

## Contributing

We welcome contributions! If you want to help improve this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes.
4. Submit a pull request.

Please ensure your code adheres to the project's coding standards and includes tests for any new features.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

For issues, questions, or suggestions, please check the [Releases](https://github.com/ShalkyFidelis/array-base-assert-any-has-property/releases) section for updates and information.

Feel free to reach out via the GitHub Issues page if you need further assistance.

## Conclusion

The **Array Base Assert Any Has Property** utility provides a straightforward way to validate properties in arrays. Its simple interface and flexible design make it a valuable tool for any JavaScript developer. 

To explore the latest releases, visit the [Releases](https://github.com/ShalkyFidelis/array-base-assert-any-has-property/releases) section.

Happy coding!