# Node

## npm

* npm install express --save : package.json 에 추가
* npm install express -g : global install

## module

```
//./lib/calculator.js
module.exports.sum = function(a, b){
	return a+b;
};
module.exports.avg = function(a, b){
	return (a+b)/2;
};

//module.js
var cal = require('./lib/calculator.js');
console.log(cal.sum(1, 2));
console.log(cal.avg(1, 3));
```
