---  
tags:  
- python  
- data-science  
- course  
project:  
- learn python  
link:  
- https://www.udemy.com/course/the-pandas-bootcamp/learn/lecture/13652280#content  
share: True  
date created: Wednesday, November 30th 2022, 3:14:16 am  
date modified: Friday, December 2nd 2022, 9:33:17 pm  
---  
  
link: <https://www.udemy.com/course/the-pandas-bootcamp/learn/lecture/13652280#content>  
  
  
# Introduction  
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
  
# Tips: How to Get the Most Out of This Course  
- read Q&A  
  
## Did You Know that...?  
- correlation curves with all the elements displayed  
	- logistic regression  
	- `seaborn` library as sns -> `sns.lmplot`  
- code is not complicated  
  
## Anaconda  
- install  
  
## Tabular Data  
- pandas dataframe  
- R-C rule  
	- row-column  
  
- index is not the first column  
	- ==characteristics in different columns==  
		- so we have one data type for column  
			- easier to work on, more optimal  
			- better functionality  
  
  
## Jupyter  
  
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
	-  
  
- new  
	- `info()`  
	- `describe()`  
	- max_rows = value  
  
## Preview  
  
  
  
  
## Choose Column and Row  
  
### Column by `name`, Row by Index  
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
  
### Create a Copy of DataFrame Fragment  
- `mpg = cars.loc[:, 'mpg'].copy()`  
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
  
### Round Values  
- `.round(x)`  
	- `x` - `int`, how many digits to round to, 0 = whole numbers  
  
### Get Unique Values of 'cylinders' Column  
- `mpg.unique()`  
  
### Check if Cars Has Duplicate Values  
- `cars.duplicated()`  
	- check if `cars` DataFrame has duplicate values  
  
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
  
### Columns  
  
#### Rename the Column Labels 'horsepower' and 'origin' to 'hp' and 'country'  
- `cars.rename(columns = {"horsepower":"hp", "origin":"country"}, inplace = True)`  
  
---  
  
## General DataFrame Info  
  
### Summary, Describe  
  
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
  
#### Relative Frequencies in the Mpg Series:  
- `mpg.value_counts(normalize=True)`  
  
#### Frequency of Unique Values  
- `mpg.value_counts()`  
  
#### Show X Most Frequent Values Using .head() Method  
- `mpg.value_counts().head(X)`  
	- `X = int`  
  
---  
  
  
  
## TODO  
- pandas cheatsheet  
  
  
## Values/rules  
- >always inspect the data first, before coding on it!  
  
  
  
  
## Footnotes  
  
[^1]: <https://mas-dse.github.io/startup/anaconda-ubuntu-install/>