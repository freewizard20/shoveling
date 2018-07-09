# Javascript basics

## REGEX

```
var test = /.js/;
console.log(test.exec('hello.js')); // [ '.js', index: 5, input: 'hello.js' ]
console.log(test.test('ghsd.js')); // true
console.log(test.test('asdasdas.cpp')); // false
```

## FILE SYSTEMS

const fs = require('fs');

var data = fs.readFileSync('./extract.js', 'utf8');

console.log(data);

fs.readFile('./extract.js', 'utf8', (err,data)=>{
    if(err) throw err;
    console.log(data);
});
```
