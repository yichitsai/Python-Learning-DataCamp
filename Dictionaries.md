# Dictionaries

```
my_dict = {
   "key1":"value1",
   "key2":"value2",
}
```

> Keys have to be "immutable objects.
> List is not immutable.Its contents can be changed after it created.

### Update the pairs
#### Add
##### Method 1:
```
my_dict = {
   "key1":"value1",
   "key2":"value2",
}

my_dict["key3"]="value3"

```
#### Method 2:
```
my_dict = {
   "key1":"value1",
   "key2":"value2",
}

dic1={"key3":"value3"}
my_dict.update(dic1)

```

#### Remove
```
del my_dict["key"] #using del to remove a dict

```

### Dictionaries of Dictionaries
```
nested_dict = { 'dictA': {'key_1': 'value_1'},
                'dictB': {'key_2': 'value_2'}}
```

```=1
Ex:
people = {1: {'name': 'John', 'age': '27', 'sex': 'Male'},
          2: {'name': 'Marie', 'age': '22', 'sex': 'Female'}}

Ask for number 1's age:
print(people[1]['age'])
```

