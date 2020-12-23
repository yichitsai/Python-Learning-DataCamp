# Python Learning
## Intro to Python

### Output
```
print(  )

  EX:print( 5 + 7 )
  Outcome: 12
```

### Add Comment
```
#Comment
```

### Arithmetic with Python
```
1. Addition: +
2. Subtraction:-
3. Multiplication: *
4. Division: /
5. Modulo: %
6. Exponentiation: **
```

### Python Type

#### To Find Out Type:
```
 type()
```
**Different Type = Different Behavior!!**


---



| Type                 | Explain                                               | Example                      |
| -------------------- |:----------------------------------------------------- | ---------------------------- |
| int/integar          | a number without a fractional part                    | 100                          |
| float/floating point | a number that has both an integer and fractional part | 100.1                        |
| str/string           | a type to represent text                              | "abcd"  or "abc"+"d" ="abcd" |
| bool/boolean         | a type to represent logical values                    | True/False                   |




---

### Type Conversion
 ```
 str()
 int()
 float()
 bool()
```
 
```1=
# Definition of savings and result
savings = 100
result = 100 * 1.10 ** 7

# Fix the printout
print("I started with $" + savings + " and now have $" + result + ". Awesome!")

#Result
Traceback (most recent call last):
  File "<stdin>", line 6, in <module>
    print("I started with $" + savings + " and now have $" + result + ". Awesome!")
TypeError: must be str, not int

#Sol:
>  savings and result type are int
>  print(string+int) ->error
>  Have to turn "int" to "str"

print("I started with $" + str(savings) + " and now have $" + str(result) + ". Awesome!")

```