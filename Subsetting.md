## Subsetting

#### 1. Index:
 Getting a specific number from a list
```=1
 grades = [88, 72, 60, 50]
           0   1   2   3
 grades[2]
 >60
 grades[0]
 >88
```

#### 2. Slicing:
 Getting a set of numbers from a list
 ```=1
 grades = [88, 72, 60, 50]
          0  1   2   3   4
 grades[0:3]
 >[88, 72, 60]
 grades[1:3]
 >[72, 60]
```


---

## Subset and Calculate
```=1
grades = [88, 72, 60, 50]

sum_grades = grades[0] + grades[2]
>148
```



---


## Slicing and Dicing
  Selecting multiple elements from your list.

#### 1. list[start,end]
```=1
grades[start,end]
grades = [88, 72, 60, 50]
grades[1:3]
>[72,60]
```
==**Start** index **included**! **End** index **excluded**!==

#### 2.list[2:] list[:]
 You have start index, but no end index.
 The computer will list from "start index" to the end.
```=1
grades = [88, 72, 60, 50]
grades[2:]
>[60, 50]

grades[:]
>[88, 72, 60, 50]
```

--- 
## Subsetting Lists of Lists :star:
 When a list inside have lists.
 ```=1
 x = [["a", "b", "c"],
     ["d", "e", "f"],
     ["g", "h", "i"]]
x[2] #第2個list of x
>["g", "h", "i"] 

x[2][0] #第2個list的第0個數字
>"g"

x[-1] #從["a","b","c"]數來倒數第0個list為始反推
>["g", "h", "i"]

x[-0] or x[-3] ＃倒數第0個開始=第0個list=
>["a", "b", "c"]
 ```

