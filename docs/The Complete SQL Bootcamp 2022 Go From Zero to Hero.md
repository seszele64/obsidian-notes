---  
tags:  
- sql  
- data  
project:  
- sql  
share: True  
date created: Wednesday, December 7th 2022, 5:59:25 pm  
date modified: Thursday, December 8th 2022, 5:35:30 pm  
link: https://udemy.toolzbuy.com/course/the-complete-sql-bootcamp/learn/lecture/19242668?courseId=762616#overview  
finished: Section 2, Video 16   
title: The Complete SQL Bootcamp 2022 Go From Zero to Hero  
aliases: [The Complete SQL Bootcamp 2022 Go From Zero to Hero]  
linter-yaml-title-alias: The Complete SQL Bootcamp 2022 Go From Zero to Hero  
---  
  
# The Complete SQL Bootcamp 2022 Go From Zero to Hero  
  
## Info  
1. Our QA forums can be found by going to your course dashboard (top right button when viewing a lecture): (<https://support.udemy.com/hc/en-us/articles/229233387-How-to-Use-The-Q-A)>  
2. Our student chat channel is here: <https://discord.gg/TztE6B8>  
3. Video guide to the chat room: <https://www.youtube.com/watch?v=bkH89OJ001M>  
4. Our PDF Notes can be found as resources in the FAQ  lecture. (<https://support.udemy.com/hc/en-us/articles/229604708-Downloading-Supplemental-Resources)>  
5. Info on certification:  <https://support.udemy.com/hc/en-us/articles/229603868-Certificate-of-Completion>  
6. Any video issues or certification issues, email: support@udemy.com  
7. Please do not direct message with questions, due to the amount of students in the course, questions are ONLY answered in the QA Forums (<https://support.udemy.com/hc/en-us/articles/229233387-How-to-Use-The-Q-A).>  
  
## Course  
- for beginners (no prior knowledge needed)  
- using PostgreSQL  
  
## Course Curriculum Overview  
  
1. installation of postgreSQL  
2. databases and tables basics  
3. sql statement fundamentals  
4. group by clause  
5. assesment test 1  
6. joins  
7. advanced sql  
8. commands  
9. assessment test 2  
10. create databases and tables  
11. assessment test 3  
12. extra lectures  
	- postresql with python  
  
  
## Database Overview  
- what are databases?  
	- dbs are systems that allow users to store and organize data  
- why use databases?  
	- useful when dealing with large amounts of data  
  
### From Spreadsheets to Databases  
  
- spreadsheets  
	- one time analysis  
	- quickly need to chart something  
	- reasonable (small) data size  
	- good for newbies  
  
- databases  
	- data integrity  
	- can handle bigger amounts of data  
	- quickly combine different datasets  
	- automate steps for re-use  
	- support for websites and applications  
		- websites and apps are linked to those dbs  
  
- database structure  
	- tables  
	- columns  
	- rows  
  
- database platform options  
	- many  
	- postgresql  
		- free  
		- open source  
		- multi platform  
		- widely used on internet  
	- mysql / mariasql  
		- free  
		- open source  
		- widely used on internet  
		- multiplatform  
	- ms sql server express  
	- microsoft access  
		- cost  
	- sqlite  
		- free  
		- open source  
		- mainly cmd  
  
- postgresql  
	- good to learn sql  
  
- sql is useful for a lot of things!  
  
  
## Install Postgresql  
  
1. install postgresql  
	- linux  
		- `sudo apt install postgresql postgresql-contrib`  
	- Ensure that the service is started:  
		- `sudo systemctl start postgresql.service`  
2. [install pgadmin](https://www.pgadmin.org/download/pgadmin-4-apt/)  
	- `curl -fsS https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo gpg --dearmor -o /usr/share/keyrings/packages-pgadmin-org.gpg`  
	- `sudo sh -c 'echo "deb [signed-by=/usr/share/keyrings/packages-pgadmin-org.gpg] https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/$(lsb_release -cs) pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list && apt update'`  
	- `sudo apt install pgadmin4`  
	- `sudo apt install pgadmin4-desktop`  
	- `sudo apt install pgadmin4-web`  
	- Apache successfully restarted. You can now start using pgAdmin 4 in web mode at <http://127.0.0.1/pgadmin4>  
3. download file "dvdrental.tar"  
	- don't open file directly, only via pgadmin  
4. restart computer  
5. restore the database  
  
  
- import database  
	- data/objects  
		- sections  
			- [x] pre-data  
			- [x] data  
			- [x] post-data  
  
  
- queries  
	- right click > query tool  
  
- select all  
	- `SELECT * FROM film`  
  
  
## Sql Statement Fundamentals  
- sql syntax  
- syntax can be applied to major types of sql database  
	- mysql, oracle  
  
### SELECT Statement  
- the most common statement  
- allows to ==retrieve== the information from a table  
  
- syntax  
	- `SELECT column_name FROM table_name`  
	- capitalize syntax statements  
		- easier to read!  
  
- inside a db you will have a few tables  
	- a table consists of rows and columns  
  
- query knows which db you use, since you open a query inside/within it  
  
- one column  
	- `SELECT c1 FROM table_1`  
- multiple columns  
	- separated by comma  
	- `SELECT c1, c3 FROM table_1`  
- all columns  
	- `SELECT * FROM table_1`  
		- ==not a good practice== to use asterisk, if you don't need all the columns  
		- it will automatically query everything, which ==increases traffic== between the database server and the applications  
  
- what tables are available to me?  
	- schemas > public > tables > expand  
  
- view whole table using query  
	- `SELECT * FROM table_name;`  
  
- semicolon at the end of the query  
	- readability  
  
- query history!  
  
### Challenge  
  
- structure  
	- business situation  
	- question  
	- expected answer  
	- hints  
	- solution  
  
- situation  
	- existing customers  
  
- challenge  
	- use `SELECT` to grab the first and last names of the existing customers, also their emails  
  
- answer  
	- `SELECT first_name, last_name, email FROM customer;`  
  
  
## SELECT DISTINCT  
- `SELECT DISTINCT`  
- sometimes there may be duplicate values in a column, thus  
	- return only the unique values in a column  
  
- syntax  
	- `SELECT DISTINCT column FROM table;`  
	- `SELECT DISTINCT(column) FROM table;`  
		- more readability  
  
- when is it useful to use `SELECT DISTINCT`?  
	- ranks  
  
### Challenge  
- situation  
	- mpaa movie ratings (pg, pg-13, R, etc.)  
	- what ratings do we have available  
  
- sql challenge  
	- retrieve unique rating types  
  
- solution  
	- `SELECT DISTINCT(rating) FROM film;`  
	- output  
```  
"PG"  
"R"  
"G"  
"PG-13"  
"NC-17"  
```  
  
  
## COUNT  
- returns the ==number of rows that match== a specific **condition** of a query  
- we can apply `COUNT` on a specific column `COUNT(column)` or just pass `COUNT(*)`  
	- output is usually the same, since all columns have the same number of rows (generally), unless we use a specific condition  
  
- syntax  
	- `SELECT COUNT(column_name) FROM table;`  
  
- combine  
	- with `DISTINCT`  
	- `SELECT COUNT(DISTINCT(column_name)) FROM table;`  
  
  
## SELECT WHERE  
- `SELECT` and `WHERE` most fundamental statements  
- `WHERE` statement allows us to specify conditions on columns for the rows to be returned  
  
### Syntax  
  
```SQL  
SELECT column1, column2  
FROM table  
WHERE conditions;  
```  
  
- `WHERE` specifies conditions  
	- conditions are used to filter the rows returned from the `SELECT` statement  
  
- appears after `FROM` clause  
- not unique to postgreSQL  
  
- compare operators  
	- compare column value to something  
		- is the price greater than $3?  
		- is the pet's name equal to "Sam"?  
  
### Operators  
- operators  
	- math operators  
		- =, >, <, >=, <=, <> or !=  
	- logical operators  
		- `AND`  
			- conjunction  
		- `OR`  
			- alternative  
		- `NOT`  
			- opposite  
  
### Examples  
- name = "David"  
	- `SELECT name, choice FROM table WHERE name = 'David'`  
		- single quotes  
		- capitalization does matter  
  
- multiple WHERE conditions  
```sql  
SELECT * FROM film  
WHERE (rental_rate > 4) AND (replacement_cost >= 19.99);  
```  
  
  
### Challenge  
- email for Nancy Thomas  
```sql  
SELECT email FROM customer  
WHERE (first_name = 'Nancy') AND (last_name = 'Thomas');  
```  
  
- description of movie 'Outlaw Hanky'  
```sql  
SELECT description FROM film  
WHERE title = 'Outlaw Hanky';  
```  
  
- phone number for customer living at `259 Ipoh Drive`  
```sql  
SELECT phone FROM address  
WHERE address = '259 Ipoh Drive'  
```  
  
  
  
## ORDER BY  
- same query may return the same results in a different order  
- you can use ORDER BY to sort rows based on a column value in either ==ascending== or ==descending== order  
