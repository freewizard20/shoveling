# python cheat sheet

## Basic Data structures
* `print("{} hello {}".format('jeon',32))`
* type check : `type(10)==int`
* List : `a = [1,2,3,4,5]` , methods : `a.append(1)` , `del a[2]`
* Dictionary : `me = {'height : 180'}` , methods : `del me['height']`
* Tuples : `a,b = (10,15)`
* Sets : `a = {1,2,3,4,5}`, has no orders, methods : `a.add(10)`, `a.discard(10)`
* Logical operators : not, or, and

## for statements
* dictionaries :
```
for x in values(): # rotate values
for v in x: # rotate keys
for i in range(len(list)): # index rotator
```

## Import statements
* statements :
```
import numpy as np
import sys
from {{filename}} import {{variables, methods}} # variables are copies not references
```
* usage : use as objects `me = lab.Man("Kim")`
* `if __name__ == '__main__'` : use to distinguish main and import
* add import directory
```
import sys
sys.path.append('../..')
```
## Methods
* methods return tuples
* 

## basic functions
* type(3) >> class 'int'
* integer division "//"
* int(), float(), round()

## OOP
righteye=lefteye 하면 같은 오브젝트를 포인팅하는거다
