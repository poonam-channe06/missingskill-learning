
 # HTML 

* HTML is HyperText Markup Language which is used to define parts of web pages or mobile apps to the web browser.


* It is the basic building block of a web development process. It is nothing but the simple tex and hyperlinks & hypertext. 

* HTML tellsbrowsers which parts of webpages is navbar ,header,footer,images and videos are placed etc.


> < !DOCTYPE html>
<p>DOCTYPE stands for document type declaration. It will simply implies that this file is going to use as HTML5 so we can load this file on the browser.</p>



<!-- images -->

<p align="center"/><img src="Images\html_1.jpg" width="400" />

 # CSS

 ### CSS Selectors :

 1. CSS Element selector
 2. CSS ID Selector
 3. CSS Group Selector
 4. CSS Class Selector
 5. CSS Universal Selector 


<p> The html selector selects the HTML element by name.</p>

 ```html
 <html>  
<head>  
<style>  
p{  
    font-size: 2rem;
    color: blue;  
}   
</style>  
</head>  
<body> 
<h1>Hello,welm to my website</h1>  
<h2 class="center"> Landing Page </h2>  
<p>This style will be applied on every paragraph.</p>  
<p id="paragraph1"> Hello World !</p>   
</body
</html>
 ```


<p> The id selector selects the id attribute of an HTML element to select a specific element. An id is always unique within the page so it is chosen to select a single, unique element. It is written with the hash character (#)</p>



```html
#paragraph1 {  
    text-align: center;  
    color: blue;  
}  
```


<p>The grouping selector is used to select all the elements with the same style definitions.Grouping selector is used to minimize the code. Commas are used to separate each selector in grouping.</p>




``` html
h1,h2,p {  
    font-family:san-serif;
    color:pink;
}  
```



<p>If we want to specify that only one specific HTML element should be affected then we should use the element name with class selector.</p>


```html
h2.center {  
    text-align: center;  
    font-size:3rem; 
}  
```

<p>It selects all the elements on the pages.</p>

```html
* {  
   line-height:1.4;
   margin:0;
   padding:0;
}   
```


####  There are 3 ways to add the CSS in our page.
1. Inline CSS
2. Internal CSS
3. External CSS

### Inline CSS :  
<p>Inline CSS is used to apply CSS on a single line or element.</p>

```html
<p style="color:blue">Hello World!!</p>  
```

### Internal CSS :
<p>Internal css apply in the single document we add the internal css in html file only inside the style tag. </p>

```html
<style>  
p{color:blue}  
</style>
```


### External CSS :
<p> It is used to apply CSS on multiple pages or all pages</p>

```html
<link rel="stylesheet" type="text/css" href="style.css">  
```

#### In external stylesheet we can  write this.
```html
p{color:blue}  
```


<p align="center"/><img src="Images\css-positionio.png" width="500" />

<p align="center"/><img src="Images\css-gridio.png" width="500" />

<p align="center"/><img src="Images\css-flexboxio (2).png" width="500" />

# SQL

* DATA : Data is  rawfact which describes the attribute of an entity.

* DATABASE : Database is place where we store the data in systematic and orgnized manner.

 
* RDBMS : Its stands for Relational database managment system. It is type of DBMS software where we store data in the form of tables and relationals.

* Relational Model : 
It is designed by data scientist EF Codd. All the data in relational model re stored in the form of tables or relations.
we can store the metadata also.

* EF Codd Rules :
-----------------------
1. Data enter into the cell should be single valued or atomic data.
2. We can store the data in multiple tables and we have to establish  the connection between those two tables using key attribute.
3.To validate the table we can assign datatype & constraints.
4. Datatype are madantory but constraints are optional.




### SQL (Structured Query Language)

> It is a language which is used to communicate with the RDBMS.

> Query Language : it is a language which is used to ciommunicate with DBMS software.


##  Types of Constraints :
---

1. NOT NULL

2. UNIQUE 

3. Primary Key 

4. Foreign Key 

5. Check



* NULL :
  * NULL is nothing, it is neither zero nor blank space
  * It will not occupy any space in the memory
  * Two NULLS are never same in Oracle.
  * NULL represents unknown value
  * Any arithmetic operation we perform on NULL will result in NULL itself. For ex, 100000 + NULL
   = NULL ; 100000 * NULL = NULL .


* NOT NULL :

  * NOT NULL will ensure atleast some value should be present in a column.




* UNIQUE :
    * It will not allow any duplicates in a column.
    * UNIQUE column can take multiple NULL (s).


* Primary Key :
  * It is the combination of NOT NULL and UNIQUE.
  * Only one PK is allowed in a table.
  * PK identifies a record uniquely in a table.
 Creation of PK is not mandatory, but it is highly recommended to create

* Foreign Key:
   * FK creates relationship between any two tables.
   * FK is also called as referential integrity constraints.
   * FK is created on the child table.
   * FK can take both NULL and duplicate values.
   * To create FK, the master table should have PK defined on the common column of the master table.
   *  We can have more than 1 FK in a given table.


   <p align="center"/><img src="Images\foreignkeyio.png" width="500" />

* CHECK:
   * It is used to provide additional validations as per the customer requirements.
    Examples; 
    1) sal > 0
    2) empnum should start with 1
    3) commission should be between 1000 & 5000





<!-- Select clause img -->
 <p align="center"/><img src="Images\select-clauseio.png" width="500" />



 <p align="center"/><img src="Images\where-clauseio.png" width="500" />


## Operators 
-------

* Operators are classified into 

1. Arithmetic Operators(+,-,*,/)
2. Relational Operators(<,>,>=,<=,<>,!=)
3. Logical Opeartors(NOT,OR,AND)
4. Special Operators(IN,NOT IN ,LIKE,NOT LIKE, BETWEEN ,IS ,IS NOT)



| EMPNO         | ENAME         |  JOB       |  MGR   |  HIREDATE  |  SAL  | COMM  | DEPTNO   |
| ------------- | ------------- | -----------| -------| -----------| ----- | ------ | ------- |
| 7369          |   SMITH       |  CLERK     |   7902 | 17-DEC-80  | 800   |       |  30      |
| 7499          |   ALLEN       |  SALESMAN  |   7698 | 20-FEB-81  |  1600 |  300  |  30      |
| 7521          |   WARD        |  SALESMAN  |   7698 | 22-FEB-81  | 1250  |  500  |  20      |
| 7566          |   JONES       |  MANAGER   |   7839 | 02-APR-81  |  2975 |       |  30      |
| 7654          |   SMITH       |  SALESMAN  |   7698 | 28-SEP-81  | 1250  | 1400  |  30      |
| 7698          |   MARTIN      |  MANAGER   |   7839 | 20-FEB-81  |  2850 |       |  10      |
| 7782          |   BLAKE       |  MANAGER   |   7839 | 07-MAY-81  | 2450  |       |  20      |
| 7788          |   CLARK       |  ANALYST   |   7566 | 09-JUN-87  |  2450 |       |  10      |
| 7839          |   SCOTT       |  CLERK     |   7566 | 19-APR-81  | 3000  |       |  10      |
| 7844          |   KING        | PRESIDENT  |        | 20-FEB-81  |  5000 |       |  30      |
| 7876          |   TURNER      |  SALESMAN  |   7698 | 23-NOV-87  | 1100  |   0   |  20      |
| 7900          |   JAMES       |  CLERK     |   7788 | 03-DEC-81  |  950  |       |  30      |
| 7902          |   FORD        |  CLERK     |   7698 | 03-DEC-81  | 3000  |       |  20      |
| 7934          |   MILLER      |  ANALYST   |   7782 | 23-JAN-82  |  1300 |       |  10      |
|               |               |            |        |            |       |       |          |

> NOTE : for all the operations we can refer this table

<p>List all the employees in department no 00 and 30</p>

```SQL
SELECT * FROM EMP 
WHERE DEPTNO IN(10,30);
```

<p>List all the employees whose name start with 'A'</p>

```SQL
SELECT * FROM EMP 
WHERE ENAME LIKE 'A%';
```


<p>List all the employees whose name IS having at least 2 Ls</p>

```SQL
SELECT * FROM EMP 
WHERE ENAME LIKE "_LL_%";
```


<P>List the employees whose salary is between 2000 and 3000</P>


```SQL
SELECT * FROM EMP 
WHERE SAL BETWEEN 2000 AND 3000;
```

<p>List all the employees whose commission is null</p>

```SQL
SELECT * FROM EMP 
WHERE COMM IS NULL;
```


### SORTING
* It arranges the data either in ascending / descending order
* Ascending – ASC / Descending – DESC
* We can sort the data using ORDER BY
* By default, the data is always arranged in ASC order
* ORDER BY should be used always as the last statement in the SQL query.


<p>Arrange all the employees by their salary</p>

```SQL
SELECT * FROM EMP 
ORDER BY SAL;
```
<p>Arrange ename, sal, job, empno and sort by descending order of salary</p>


```SQL
SELECT ENAME,SAL,JOB,EMPNO
 FROM EMP 
ORDER BY 2 DESC;
```

>NOTE: In the above query we have – order by 2 – thus it arranges only the 2nd column salary in the DESCENDING ORDER.




## Functions :



<p align="center"/><img src="Images\functionio.png" width="500" />



### Single Row Functions :

| SRF                       | Explanation   | 
| -------------             |  ------------- | 
| UPPER('STR')              |  To obtain the output in the uppercase  eg. SELECT UPPER('poonam')  FROM DUAL;                  |
| INITCAP('STR')            |  It is used to obtain all the letters in lowercase but first letter in uppercase.                           |
| REVERSE('STR')            |  It is used to obtain the string in reverse.      |
| LENGTH('STR')             |  It is used to obtain number of character present in the string.                     |
|SUBSTR('original string',position[,length]); | It is used to obtain string from given original string.            |
| REPLACE                   |  It is used to replace sub string with new string.   |
| INSTR('original string','sub-string',position[,Nth occurance]);  | It is used to obtain index value or osition of the substring in which iit is present in the original string.        |
| MODULUS                   |  Used to obtain reminder.             |
|  TO_CHAR                  |  It is used to convert given date format into char format.                                                        |
|  SELECT TO_CHAR(SYSDATE,'YYYY')   
|  SELECT TO_CHAR(SYSDATE,'YEAR')
|  SELECT TO_CHAR(SYSDATE,'YY')
|  SELECT TO_CHAR(SYSDATE,'MON')
|  SELECT TO_CHAR(SYSDATE,'MONTH')
|  SELECT TO_CHAR(SYSDATE,'MM')
| SELECT TO_CHAR(SYSDATE,'DAY')
| SELECT TO_CHAR(SYSDATE,'DD')
| SELECT TO_CHAR(SYSDATE,'YY')
| SELECT TO_CHAR(SYSDATE,'DY')
|                                                                     |

  



## Multirow Functions :

| MRF           | Syntax                        | Explanation          |
| ------------- | -------------                 | --------------       |
| MAX           | MAX(COLNAME OR EXPRESSION)    |  It is used to obatin the maximun value. eg MAX(SAL).
| MIN           | MIN(COLNAME OR EXPRESSION)    |  It is used to obatin the smallest value. |
| SUM           | SUM(COLNAME OR EXPRESSION)    |  It is used to obtain sum of values.      |
| AVG           | AVG(COLNAME OR EXPRESSION)    | It is used to obtain average of the values.||
| COUNT         | COUNT( * / COLNAME OR EXPRESSION) | It is used to obtain number of values.  |
|               |                                   |                                         |





## SUBQUERY :

<p align="center"/><img src="Images\subquery_1.jpg" width="500" />


* When do we go for Subquery?
<p> 1. When we have unknown values we will go for subquery.</p>
<p> 2. When data to be display is in one table but condition present in another table then we will go for subquery.</p>


* Conditions to write Subquery?
<p> 1. Only one column should be return in select clause of inner query.</p>
<p> 2. Column name of SELECT clause in inner query and column name of WHERE clause of outer query should have same data type .</p>



* Types of Subquery:
 1. Single row subquery : If inner query of subquery giving single input to outer query then it is called as single row subquery.(=,>,<,>=,<=)

 2. Multirow subquery : If the inner query of subquery giving multiple input to outer query then it is called as multirow subquery.(In,NOT IN)
 





## JOINS :

* Retrival of data from multiple table simulteneously is called as joins.

<p>There are five types of joins</p>
1. Cartesian join or Cross join

2. Inner join/Equi join

3. Natural join

4. Outer join

5. Self join



1] CARTESIAN JOIN : All the records of table 1 merge with records of table 2.

Syntax:
```SQL
SELECT COL-NAME FROM T1,T2; // Oracle 
```

```SQL
SELECT COL-NAME FROM T1 CROSS JOIN T2; // ANSI
```
<p align="center"/><img src="Images\cartesianjoin.png" width="500" />

2] INNER JOIN : It is used to get matched records.

Syntax:
```SQL
SELECT COL-NAME FROM T1,T2 
WHERE < JOIN CONDITION >; // Oracle 
```

```SQL
SELECT COL-NAME FROM T1 INNER JOIN T2 
WHERE < JOIN CONDITION >; //ANSI
```

<p>Join condition is where two tables are merged.</p>
<P>T1.COL-NAME = T2.COL-NAME</P>

<!-- JOIN COONDITION IMAGES -->
<p align="center"/><img src="Images\innerjoin.png" width="500" />


3] NATURAL JOIN : It is same as the inner join but here we no need to write the join condition.

Syntax:

```SQL
SELECT COL-NAME FROM T1 NATURAL JOIN T2; // ANSI 
````


4] OUTER JOIN: Whenever we want matched records along with the unmatched records we will go for outer join.

* Types of Outer join:
 1. left outer join
 2. right outer join
 3. full outer join

 1] Left outer join : To obtain matched records along wth unmatched records of left table.
 Syntax:

 ```SQL
 SELECT COL-NAME FROM T1,T2
 WHERE T1.COL-NAME = T2.COL-NAME(+); //ORACLE
 ```

 ```SQL
 SELECT COL-NAME FROM T1 LEFT OUTER JOIN T2
 WHERE T1.COL-NAME = T2.COL-NAME; // ANSI
 ```
<!-- LEFT OUTER DIAGRAM -->
<p align="center"/><img src="Images\outerjoin.png" width="500" />

2] Right outer join : To obtain matched records along wth unmatched records of right table.

 Syntax:

 ```SQL
 SELECT COL-NAME FROM T1,T2
 WHERE T1.COL-NAME(+) = T2.COL-NAME; //ORACLE
 ```

 ```SQL
 SELECT COL-NAME FROM T1 RIGHT OUTER JOIN T2
 WHERE T1.COL-NAME = T2.COL-NAME; // ANSI
 ```


3] Full outer join : To obtain matched records along wth unmatched records of both the table.

 Syntax:

 ```SQL
 SELECT COL-NAME FROM T1 FULL OUTER JOIN T2
 WHERE T.COL-NAME = T2.COL-NAME; // ANSI
 ```



5] SELF JOIN : Joining two same table is called as self join.

#### When we go for self join ?
<p>Whenever data present in the same table but they are in different rows.</p>

Syntax:  

```SQL
SELECT COL-NAME FROM T1,T2
WHERE T1.COL-NAME =  T2.COL-NAME; // ORACLE
```

```SQL
SELECT COL-NAME FROM T1 JOIN T2
WHERE T1.COL-NAME =  T2.COL-NAME; // ANSI
```

<p align="center"/><img src="Images\selfjoin.png" width="500" />

## DEPENDANCY : 

<p align="center"/><img src="Images\dependancy_1.jpg" width="500" />


## NORMALIZATION :

#### What are the Normalization ?

<p>
 It is the procees of reducing larger tables into smaller table by indentifying dependancy to avoid redundancy and anomaly.

 The databse normalization is structured way to decompose the data to eliminate the redundancy and undesirable anomaly.
<p/>

>Redundancy: Repetition of the data or unwanted data.

>Anomaly : Side effects caused by the repetiotion called as anomaly.


<!-- IMAGES -->

<p align="center"/><img src="Images\normalform_1.jpg" width="500" />

<p align="center"/><img src="Images\normalform2_1.jpg" width="500" />

