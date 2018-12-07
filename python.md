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
* `def(opic=True, flat)` : default values in method, order is not relevant.

## basic methods
* type(3) >> class 'int'
* integer division "//"
* int(), float(), round()

## Classes
```
class Man:
  def __init__(self,...):
    self.name = name
    # we need to initialize all class variables here
    
  def hello(self,...):
```

* usage:
```
me = Man("Kim")
me.hello() # omit the self here
```

## Pickles
```
import pickle
f = open(‘data.pkl’, ‘wb’)
pickle.dump({{오브젝트}}, f)
f = open(‘data.pkl’, ‘rb’)
{{오브젝트}} = pickle.load(f)
# objects queued inside pkl file.
```

## Copy
```
import copy
b = copy.deepcopy(a)
```

## numpy
### making numpy arrays
* `np.array([1,2,3])` : make a array
* `np.arange(0.5,0,1)` : [0,5) array with 0.1 interval


## Anaconda
* `conda create --name {{envname}} python=3.6`
* `conda env list`
* `source activate {{envname}}`
* `conda list --explicit > bio-env.txt`
* `conda env create --file bio-env.txt`
