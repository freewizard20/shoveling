# Javascript basics

## REGEX

```
var test = /.js/;
console.log(test.exec('hello.js')); // [ '.js', index: 5, input: 'hello.js' ]
console.log(test.test('ghsd.js')); // true
console.log(test.test('asdasdas.cpp')); // false
