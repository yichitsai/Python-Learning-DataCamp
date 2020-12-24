## Difference between Remove, Delete,and Pop

### list.remove(value)
#### Remove the first matching object/value. Does nothing to the index.

```=1
my_list = [1,2,3,2]
my_list.remove(2)  #value:2

my_list
>[1,3,2]
```

### del list[index]
#### Removes the item at a specific index.
```
my_list = [1,2,3,2]
del my_list[2] #位置第3個

my_list
>[1,2,2]
```

### list.pop(index)
#### Removes the item at a specific index and returns it.
```
my_list = [1,2,3,2]
pop.my_list(2) #位置第3個

my_list
>[1,2,2]
```


---

### Differences

#### 1 .remove VS  del and pop

> .remove():delete matching object/value.
> .del() and .pop():delete element at a specific index.

#### 2. del VS pop

> Both deals with the index.
> del: does not return.
> pop: delete and return.

#### 3. Object/Value VS Location
> Object/Value: remove
> Location: del or pop

#### 4. Best Way
> remove: If you want to delete a specific object in the list.
> del: If you want to delete the object at a specific location (index) in the list.
> pop: If you want to delete and get the object at the specific location.