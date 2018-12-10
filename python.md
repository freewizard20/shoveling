# python cheat sheet

## Basic Data structures
* `print("{} hello {}".format('jeon',32))`
* type check : `type(10)==int`
* List : `a = [1,2,3,4,5]` , methods : `a.append(1)` , `del a[2]`
* Dictionary : `me = {'height : 180'}` , methods : `del me['height']`
* Tuples : `a,b = (10,15)`
* Sets : `a = {1,2,3,4,5}`, has no orders, methods : `a.add(10)`, `a.discard(10)`
* Logical operators : not, or, and

## List
* `list('ABCD') # ['A','B','C','D']`

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
* run as __main__ : `python3 -m lab.lab2.lab21 # exclude the .py`
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
* toString method
```
  def __str__(self):
    return self.name
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
* `a.reshape(3,3,3)` : reshape array to new dimension

### Operations
* `+ - * /` : done by each element
* `np.sum(arr)` : list total
* `np.abs(arr)` : abs
* `np.maximum(arr1,arr2)` : returns arr3 with max elements

### Random
* `np.random.randint(5)` : 0~4 one number pick
* `np.random.randint(2,5)` : 2~4 one number pick
* `np.random.randint(2,5,10)` : 2~4 ten numbers pick
* `np.random.randint(2,5,(2,5))` : ten numbers pick of [2,5]
* `np.random.randn()` : N(0,1) standard normalized distribution
```
np.random.randn() * sigma + mean # N(mean,sigma^2)
np.random.randn(2,4) # pick of [2,4] array
```

## Plotting
```
import matplotlib.pyplot as plt
import seaborn as sns
sns.set(style="darkgrid")
tips = sns.load_dataset("tips")
sns.relplot(x="total_bill",y="tip",data=tips)
plt.show()
```

## Subprocess
```
from subprocess import check_output
print(check_output(["ls","."]).decode("utf8")
```

## Pandas
* `import pandas as pd`
* [documentation](https://pandas.pydata.org/pandas-docs/stable/10min.html)
* [dataframe](https://pandas.pydata.org/pandas-docs/version/0.23.4/generated/pandas.DataFrame.html)
* pandas dataframe to numpy : `df = df.values`
* numpy to dataframe : `df = pd.DataFrame(np.array([1,2,3]))`
* interact with CSVs : `df.to_csv('{{filename}}.csv')`, `df = pd.read_csv('{{dirname}}')`

## Anaconda
* `conda create --name {{envname}} python=3.6`
* `conda env list`
* `source activate {{envname}}`
* `conda list --explicit > bio-env.txt`
* `conda env create --file bio-env.txt`

## Notable random facts

