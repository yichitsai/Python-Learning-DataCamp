# Pandas
### High level data manipulation tool!
### Build on NumPy
### An open source library, providing high-performance, easy-to-use data structures 

---


```
keys : column labels
values : data, column by column 
```
```
import pandas as pd
```


---
## DataFrame
### A way to store tabular
#### Method 1
```
import pandas as pd
DataFrame name = pd.DataFrame(data=None, index=None, columns=None, dtype=None, copy=False)

#change data into dataframe and named a new name
```
```=1
Ex:
import pandas as pd
my_dict = {'country':'names','drives_right':'dr}

# Build a DataFrame cars from my_dict: cars
cars = pd.DataFrame(my_dict)

```

 ![](https://i.imgur.com/2xc5i7N.png) 

### Change row labels

```
DataFrame.index = labels

#labels are defined by myself

```
```=1
cars_dict = { 'country':names, 'drives_right':dr, 'cars_per_cap':cpc }
cars = pd.DataFrame(cars_dict)
#cars is a dataframe

# Definition of row_labels
row_labels = ['US', 'AUS', 'JPN', 'IN', 'RU', 'MOR', 'EG']

cars.index = row_labels
```
![](https://i.imgur.com/KPgM20w.png)

## CSV
### "Comma-Separated Values"
#### To import CSV data into Python as a Pandas DataFrame
#### Supports optionally iterating or breaking of the file into chunks.

```
pandas.read_csv()
```

```=1
# Import pandas as pd
import pandas as pd

# Import the cars.csv data: cars
cars = pd.read_csv('cars.csv') 
# Print out cars
print(cars)
```
![](https://i.imgur.com/AB6HMhK.png)

#### Make first column to Row Labels
```=1
# Fix import by including index_col
cars = pd.read_csv('cars.csv',index_col=0)
```


---
## Square brackets
```
Column access:brics[["country","capital"]]
Row access:brics[1:4]
```
### 1.Columns
#### (1).Single square bracket:Pandas series
```=1
# Print out country column as Pandas Series
cars['country']
```
![](https://i.imgur.com/umux4S1.png)

#### (2).Double square brackets:Pandas DataFrame
```=1
# Print out country column as Pandas DataFrame
cars[['country']]
cars[['country','drives_right']]
```
![](https://i.imgur.com/JIuy0jw.png)

![](https://i.imgur.com/8iXgzi9.png)
### 2. Rows
#### Using the integer indexes of the rows here, not the row labels!
```
cars[start,end]
#start:include
#end:exclude
```
```=1
# Print out first 3 observations
print(cars[0:3])
```
![](https://i.imgur.com/YFfuP1O.png)

---


## loc
### Label-based
```
Column access:brics.loc[["RU","IN","CH"]]
Row access:brics.loc[:,["country","capital"]]
Column and Row access:
           brics.loc[
           ["RU","IN","CH"],
           ["country","capital"]]
```
#### 1.Series:
```=1
#To print the resulting Series
print(cars.loc['JPN'])
```
![](https://i.imgur.com/jRU9MNn.png)
#### 2.DataFrame:
```=1
#To print the resulting DataFrame
print(cars.loc[['JPN']])
```
![](https://i.imgur.com/HV8cBMl.png)

---

## iloc
### Integer position-based
```
Column access:brics.iloc[[1,2,3]]
Row access:brics.iloc[:,[0,1]]
Row and Column access:
           brics.iloc[[1,2,3],[0,1]]
```

![](https://i.imgur.com/BqRg8FK.png)

```=1
Column access:
cars.iloc[[1,2]]
#start:include
#end:include
```
![](https://i.imgur.com/T3qbj6E.png)
```=1
Row access:
cars.iloc[:,[2]]
```
![](https://i.imgur.com/ZnRZEM4.png)
```
Row and Column access:
cars.iloc[:,[0,2]]
```
![](https://i.imgur.com/YIChUNC.png)
