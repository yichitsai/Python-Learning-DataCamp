## Methods
#### Functions that belong to objects
> #### Everything = Object
> #### Object have methods associated, depanding on type
> #### Type, such as:string,list.....
> #### Same methods may be used at different type! Behave differently!


---

### String Methods
```
str.method()
```

#### upper()
##### Change small letter to big letter
```=1
str.upper("poolhouse")
>POOLHOUSE

```

#### count()
##### Count the number of times of the character in the string 
#### 字串裡出現某字符的次數
```
str.count(sub, start, end=len(string))
#sub=character
#start= the number one character
#end= the last one character
```

```=1
place = ["Taiwan"]
place.count(sub="a")
or place.count("a",0,6)
>2
```


---

### List Methods

#### index()
##### To get the index of the first element of a list that matches its input.
##### 找出在列表中某個值的第一個匹配項的位置

```
list.index(x,[,start[,end]])
```

```=1
numbers = [11.25, 18.0, 20.0, 10.75, 9.50]
print(number.index(20))
>2
```

#### append()
##### Adds an element to the list it is called on.
##### 在末尾

```
list.append(obj)
```

#### remove()
##### Removes the first element of a list that matches the input.

```
list.remove(obj)
```


#### reverse()
##### Reverses the order of the elements in the list it is called on.

```
list.reverse(obj)
```

```=1
areas = [11.25, 18.0, 20.0, 10.75, 9.50]
areas.reverse()
>[ 9.5, 10.75, 20.0, 18.0, 11.25]
```

