# prime-checker

A lightweight CommonJS module that checks whether a number is prime.

## Usage

```js
const { isPrime } = require('prime-checker');

isPrime(7);   // true
isPrime(11);  // true
isPrime(1);   // false
isPrime(9);   // false
```

## How it works

Numbers below 2 and non-integers are rejected immediately. For everything
else, the function only tests divisors up to the square root of the input.
Any factor larger than the square root must pair with a smaller one, so
checking beyond that point is redundant.

Built while working through the freeCodeCamp Back End Development and APIs
certification.

## License

MIT
