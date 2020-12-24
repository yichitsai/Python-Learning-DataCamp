### Numpy

####  》提供非常高效能的多維陣列(multi-dimensional array)數學函式庫
####  》方便有用的線性代數(Linear Algebra)及傅立葉轉換(Fourier Transform)能力
####  》利用NumPy Array替代Python List
####  》可定義任意的數據型態(Data Type)，使得能輕易及無縫的與多種資料庫整合



---
```
import numpy as np
```
```
type()
>numpy.ndarray
```

```=1
np.array()
```

```=1
np.array([True, 1, 2]) + np.array([3, 4, False])
#True=1 ; False=0
>[4, 5, 2]
```



---
### Compare List and Numpy
#### Numpy only contains one type!
```
height = [1.73, 1.68, 1.71, 1.89, 1.79]
weight = [65.4, 59.2, 63.6, 88.4, 68.7]
weight / height ** 2
```
TypeError: unsupported operand type(s) for **: 'list' and 'int'

```
np_height = np.array(height)
np_weight = np.array(weight)
np_weight / np_height ** 2
```
```
array([ 21.852,  20.975,  21.75 ,  24.747,  21.441])

```



---
### Numpy Add VS List Add
#### Different types Different behavior!
```=1
list = [1,2,3]
np_list = np.array[1,2,3]
```
```=1
list + list
>[1,2,3,1,2,3]

np_list + np_list
>[2,4,6]
```



---


### Subsetting NumPy Arrays

```=1
np_list = np.array[1,2,3]
np_list[1]
>2

np_list >2
>[False, False, True]

np_list[np_list>2]
>3

```