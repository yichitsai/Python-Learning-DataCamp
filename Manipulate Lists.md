## Manipulating List
### Replace
```=1
x = ["a", "b", "c", "d"]
x[1] = "r"

print(x)
>["a", "r", "c", "d"]

```

### Extend
```=1
x = ["a", "b", "c", "d"]
y = x + ["e"]

print(y)
>["a", "b", "c", "d", "e"]
```

### Delete
```
del()
```
```=1
x = ["a", "b", "c", "d"]
del(x[1])

print(x)
>["a", "c", "d"]
```
### Place Commands on the same line
```
Command1; Command2
```
```=1
# Same line
command1; command2

# Separate lines
command1
command2
```
### Inner Working
 Create copied list and change the element of copied list
 Instead of changing the original list
 
 ==Correct Way==
 #### 1. [:]
 ```=1
 # Create list areas
areas = [11.25, 18.0, 20.0, 10.75, 9.50]

# Create areas_copy
areas_copy = areas[:]
 ```
 #### 2.list()
 ```=1
 # Create list areas
areas = [11.25, 18.0, 20.0, 10.75, 9.50]

# Create areas_copy
areas_copy = list(areas)
 ```
 
 ==Wrong Way==
 ```=1
 # Create list areas
areas = [11.25, 18.0, 20.0, 10.75, 9.50]

# Create areas_copy
areas_copy = areas
 ```