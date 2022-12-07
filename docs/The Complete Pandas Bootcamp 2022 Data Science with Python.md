---  
tags:  
- python  
- data-science  
- course  
- pandas  
- skills  
project:  
- learn python  
link:  
- https://www.udemy.com/course/the-pandas-bootcamp/learn/lecture/13652280#content  
share: True  
date created: Wednesday, November 30th 2022, 3:14:16 am  
date modified: Wednesday, December 7th 2022, 3:38:48 pm  
---  
  
- link: <https://www.udemy.com/course/the-pandas-bootcamp/learn/lecture/13652280#content>  
- toolz: <https://udemy.toolzbuy.com/course/the-pandas-bootcamp/learn/lecture/12579754#overview>  
  
# The Complete Pandas Bootcamp 2022 Data Science with Python  
  
- [ ] `df.info()`  
- [ ] `df.describe()`  
- [ ] `df.max_rows = `  
- [ ] pandas cheatsheet  
  
  
## Rules  
- >always inspect the data first, before coding on it!  
  
## Introduction  
- in reality you need skills in pandas, since most of the time you spend manipulating data  
- practice  
	- >150 exercises  
	- 2 final projects  
  
- use cases  
	- ML  
	- finance -> trading  
  
- use newest version of pandas, python  
	- pandas is seriously automated  
	- you need to have full picture of pandas  
  
### Tips: How to Get the Most Out of This Course  
- read Q&A  
  
### Did You Know that...?  
- correlation curves with all the elements displayed  
	- logistic regression  
	- `seaborn` library as sns -> `sns.lmplot`  
- code is not complicated  
  
### Anaconda  
- install  
  
### Tabular Data  
- pandas dataframe  
- R-C rule  
	- row-column  
  
- index is not the first column  
	- ==characteristics in different columns==  
		- so we have one data type for column  
			- easier to work on, more optimal  
			- better functionality  
  
  
### Jupyter  
  
- install jupyter  
	- `sudo apt install python3-pip python3-dev`  
	- `sudo -H pip3 install --upgrade pip`  
  
### Anaconda  
- update anaconda  
	- `conda update --all --yes`  
  
### Start  
- Start Jupyter Notebook  
	-  `jupyter notebook`[^1]  
  
- the token needed to connect to jupyter notebook via vscode is printed in the terminal  
  
  
## Pandas Cheatsheet  
- [pydata.org cheatsheet](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)  
- <https://www.dataquest.io/blog/pandas-cheat-sheet/>  
  
## Pandas Series  
- It is a one-dimensional array holding data of any type.[^2]  
- ![Pandas Series](https://media.geeksforgeeks.org/wp-content/uploads/dataSER-1.png)  
  
### Create Pd Series  
  
#### From Scratch  
- `pd.Series(values_list, index_values_list)`  
	- example  
		- `pd.Series([20, 25, 10, 0, 2, 16], index=['Mon', 'Tue', 'Wed', 'Thu', 'Fri'])`  
		- **values_list** = `[20, 25, 10, 0, 2, 16]`  
		- **index_values_list** = `['Mon', 'Tue', 'Wed', 'Thu', 'Fri']`  
  
#### From Dictionary  
- from dictionary -> Key/Value Objects as Pandas Series  
	- keys of the dictionary become the labels  
	- To select only some of the items in the dictionary, use the `index` argument and specify only the items you want to include in the Series.  
  
```python  
calories = {"day1": 420, "day2": 380, "day3": 390}    
myvar = pd.Series(calories)  
```  
  
#### From List  
```python  
a = [1, 7, 2]  
myvar = pd.Series(a)  
```  
- source[^3]  
  
#### From Numpy Array  
- `pd.Series(numpy_array)`  
  
### Convert Pandas Series to Dataframe  
- `series.to_frame()`  
	- `series` - series name  
  
---  
  
## Choose Column and Row  
  
### Select Column by `name`, Row by Index  
- single iloc  
	- choose the `['name']` of column and `.iloc[index]` of row  
		cars['name'].iloc[393]  
  
### Select Element of the Cars DataFrame  
- `cars.iloc[r,c]`  
	- `r` - row number  
	- `c` - column number  
  
### Slice  
- subset elements of a dataframe  
  
#### The Last X Rows  
- `cars.iloc[:,-1:X]`  
	- from `-1` row to `-X`th row  
  
#### Print the Last Y Columns  
- `cars.iloc[-1:X, :]`  
	- from `-1` column to `-x`th column  
  
#### Columns  
  
##### Rename Columns  
- rename the Column Labels 'horsepower' and 'origin' to 'hp' and 'country'  
	- `cars.rename(columns = {"horsepower":"hp", "origin":"country"}, inplace = True)`  
  
- Rename by mapping old names to new names using a dictionary, with form `{“old_column_name”: “new_column_name”, …}`  
	- `data = data.rename(columns={"Area": "place_name"})`  
	- `data.rename(columns={"Area": "place_name"}, inplace=True)`  
  
- Rename by providing a function to change the column names with. Functions are applied to every column name.  
	- `data.rename(columns=str.lower)`  
  
  
##### Choose Columns  
- using a dot notation, e.g. `data.column_name`  
- using square braces and the name of the column as a string, `e.g. data['column_name']`  
- using numeric indexing and the iloc selector -> `data.iloc[:, <column_number>]`[^4]  
  
#### Rows  
  
- numeric row selection using the iloc selector,  
	- `data.iloc[0:10, :]` - select the first 10 rows.  
  
- label-based row selection using the loc selector (this is only applicably if you have set an “index” on your dataframe  
	- `data.loc[44, :]`  
  
- logical-based row selection using evaluated statements,  
	- `data[data["Area"] == "Ireland"]`  
		- select the rows where Area value is ‘Ireland’.  
  
  
---  
  
### Conditions  
  
- one condition  
	- two commands  
		- set **condition**  
			- `mask1 = cars['origin'] == 'europe'`  
		- subset all cars for cars from europe, based on **condition**  
			- `europe  = cars[mask1]`  
	- one command  
		- `mask1 = cars.loc[(cars['origin'] == 'europe')]`  
  
- **two conditions**  
	- subset for two conditions: **`origin` from europe** and **`mpg` smaller than 20**  
		- `europe_le = cars.loc[(cars['origin'] == 'europe') & (cars['mpg'] < 20)]`  
	- mpg between 10 and 15, inclusive  
		- `mpg_10_15 = cars.loc[(cars['mpg'] >= 10) & (cars['mpg'] <= 15)]`  
  
---  
  
  
---  
  
### Create a Copy of DataFrame Fragment  
- `mpg = cars.loc[:, 'mpg'].copy()`  
	- mpg - pandas series  
- `origin = cars.loc[:, 'origin'].copy()`  
  
## Sort  
#operations  
  
### Sort Mpg Series in **Ascending Order**  
- `mpg_ascending = mpg.sort_values(ascending = True)`  
	- `ascending = True`  
		- ascending order, low to high  
  
### Sort High to Low, `inplace = True`  
- mpg.sort_values(ascending = False, inplace = True)  
	- `inplace = True`  
		- replace original series  
	- `ascending = False`  
		- descending order, high to low  
  
## Values  
  
### Change Single Value in Pandas Series  
- change by providing **index label** name - `series['index_label']`  
	- `sales["Sun"] = 0`  
		- sales - pandas series  
		  Sun - index label  
  
- change with `series.iloc` method  
	- `sales.iloc[3]`  
		- change value of **third row** in **sales** pandas series  
  
### Round Values  
- `.round(x)`  
	- `x` - `int`, how many digits to round to, 0 = whole numbers  
  
### Get Unique Values  
- return the unique values  
- `series.unique()`  
  
### Get Number of Unique Values  
- Return the **number of unique values** for series  
	- number of different values  
	- overlapping values are all counted as one  
- `series.nunique()`  
  
  
### Check if Pandas Series Has Duplicate Values  
- check if `series` pandas series has duplicate values  
- `series.duplicated()`  
  
### Largest/Highest/Biggest And Smallest Values in Dataframe  
  
>Protip!  
>- combine with `.loc` notation  
>	- example: `titanic.loc[titanic.age.idxmin()]`  
>	- returns row with lowest age value  
  
#### Largest Values  
- `age.nlargest(n)`  
	- n = 5 (default), choosing how many of the largest values return  
- `series.idxmax()`  
	- returns the row **index** label of the maximum value  
  
#### Smallest Values  
- `age.nsmallest(n)`  
	- n = 5 (default), choosing how many of the smallest values to return  
- `series.idxmin()`  
	- returns the row **index** label of the minimum value  
		- used to get id for the minimum value, handy since index column is unique  
  
  
### Index  
- `cars.index`  
	- `cars` - name of DataFrame  
  
#### Set 'name' Column as Index  
- `cars.set_index('name', inplace=True)`  
	- `name` - name of the column  
- `inplace = True`  
	- change original values  
  
#### Set Name of the Index to car_model  
- `cars.index.name = 'car_model'`  
	- change index column name to `'car_model'`  
  
#### Reset Index to RangeIndex and Save it to Cars  
- `cars.reset_index(inplace=True)`  
	- `inplace = True`  
		- change original value  
  
  
## Index Object  
- [pandas docs](https://pandas.pydata.org/docs/reference/indexing.html)  
- specific, have their own methods and attributes  
- ==immutable==  
  
- `.axes`  
	- range of the index (how many rows)  
	- names of the index label (names of the columns)  
  
- `.columns`  
	- `index.columns`  
	- slice columns  
		- slice the three first columns  
			- `index.columns[:3]`  
  
- `series.index.is_unique`  
	- does index have only unique values?  
		- `True` / `False`  
  
### Creating Index Object  
- `pd.Index()`  
  
- examples  
	- index values from 1 to 4  
		- `pd.Index(range(1,4))`  
	- index as weekdays  
		- pd.Index(["Mo", "Tue", "Wed", "Thu", "Fri"], name = "days")  
  
### Reset Index  
- `df.reset_index()`  
	- reset index of series/dataframe  
- `df.reset_index(drop = True)`  
	- remove the index column altogether from dataframe/series  
  
### Set Index  
- `df.set_index("Column_name")`  
  
- `df.set_index("Column_name", drop = boolean (True), inplace = boolean (True))`  
  
### Check Index Size  
- `df.index.size`  
  
### Change Index Name  
- `df.index.name`  
  
### Rename Index, Column Labels  
  
#### Mapper  
- `df.rename(mapper = dict, axis = "index")`  
  
#### Index  
- `df.rename(index = dict)`  
  
#### Rename Column Names  
- `df.rename(columns = {"Previous_col_name1":"Desired_col_name1"})`  
  
## General DataFrame Info  
  
### Summary, Describe  
  
- [ ] `df.info()`  
- [ ] `df.describe()`  
- [ ] `df.max_rows = `  
  
#### First X Rows  
- `df.tail(X = 5)`  
	- if X is None -> 5  
  
#### Last X Rows  
- `df.head()`  
	- if X is None -> 5  
  
#### Summary Statistic  
- `cars[cars.mpg.min() == cars.mpg]`  
  
#### Describe Non-numeric Column 'origin'  
- `origin.describe()`  
  
### Frequencies  
- number of occurrences, sorted from most frequent to least frequent  
	- how many X values appear in the series  
  
- `df.value_counts(sort = True, dropna = True, ascending = False, normalize = False)`  
	- `normalize` -> use relative frequencies (% of all items), sums up to 1  
  
#### Frequency of Unique Values  
- `mpg.value_counts()`  
  
#### Show X Most Frequent Values Using .head() Method  
- `mpg.value_counts().head(X)`  
	- `X = int`  
  
---  
  
### Importing Data  
  
- importing from csv  
	- `pd.read_csv("name.csv", usecols = ['column_name'])`  
		- `usecols` - select only those columns  
  
  
  
  
  
  
## TODO  
- [ ] pandas cheatsheet  
  
  
  
## Footnotes  
  
[^1]: <https://mas-dse.github.io/startup/anaconda-ubuntu-install/>  
[^2]: [Python Pandas DataFrame load, edit, view data](https://www.shanelynn.ie/using-pandas-dataframe-creating-editing-viewing-data-in-python/)  
[^3]: [Pandas Series - w3](https://www.w3schools.com/python/pandas/pandas_series.asp)