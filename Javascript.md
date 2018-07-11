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

## ES6 import 

1. import express from 'express' : npm module import, import as object template
2. import {square, diag} from './test.js' : import (export function from external file) > use directly!
3. import * as {{whatever}} from 'lib' : create instance directly as {{whatever}}

## 즉시 실행하는 어노니머스 함수 셋
```
({{async}}()=>{
    
    // function..
   
})();
```
