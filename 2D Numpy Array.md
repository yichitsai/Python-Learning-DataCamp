## 2D Numpy Array
### 2 Dimentional Array

```
object.shape
```
```=1
np_list = np.array([1.73,1.62,1.35,1.41,1.22],
                   [65.4,70.1,66.7,65.7,33.4])
np_list.shape
>(2,5) # 2 rows and 5 columns
```

==Only for one type!==

```=1
x = np.array([[1, 2, 3], [4, 5, 6]], np.int32)
type(x)
<class 'numpy.ndarray'>
```


---
### Average
```
np.mean()
```

```=1
import numpy as np
np_city = array([[1.64, 71.78], 
                 [1.37, 63.35],
                 [1.6 , 55.09],
                      ...,
                 [2.04, 74.85],
                 [2.04, 68.72],
                 [2.01, 73.57]])
                 
np.mean(np_city[:,0]) #All Rows and Column 1
>1.7472

```

### Median
```
np.median()
```
### Standard Deviation
```
np.std()
```
### Correlation
```
np.corrcoef(object1,object2)
```



---
### Subsetting
```
          0       1       2       3       4
array([[1.73,   1.68,   1.71,   1.89,   1.79],    0 
       [  65.4,   59.2,   63.6,   88.4,   68.7]]) 1
       
```
#### 1.
```
np_2d[0]
>array([ 1.73,  1.68,  1.71,  1.89,  1.79])
```
#### 2.
```
np_2d[0][2]
>1.71
```
#### 3.
```
np_2d[:,1:3] #All rows and Column 2 to Column 3
>array([[  1.68,  1.71],
        [ 59.2 , 63.6 ]])
```

