
# Basic building Block of Web Development


## IP  

* IP stands for Internet Protocol.

* Internet protocol is the communications protocol that is address assigned to each device to connected to the network.

* Data is divided into the small pieces called 'Packet'.

<!-- image of Ip address  -->

<p align="center"/><img src="Images\web_1.jpg" width="60%" />
<p align="center"/><img src="Images\web2_1.jpg" width="60%" />


<!-- Ipv4 vs Ipv6 -->
<!-- Image -->
<p align="center"/><img src="Images\ipv4v6_1.jpg" width="60%" />


<!-- Port Number -->
## Port Number

* Port number related to to the network addressing.
*Port Number, which helps to get connected with a particular server.



 ### Server 

 <p> A server is a hardware and software devices which bascially take a request from thhe client or user and give it back to response.</p>

 ### Web server

 <p>Websites is a collection of web pages while web server is a software that respond to the request for the resources. </p>


<!-- HTTP Verbs -->
## HTTP Verbs


 > HTTP verb nothing but the set of requests methods to indicate the action to be performed for the given resource.

| Methods       | Description                              |
| ------------- | -------------                            |      
| POST          | It is used to send a data to the server. eg.Uploading a file.                                                       |
| GET           | It is used to retrive the information from the server using given URL.                                                  |
| PUT           |  It is used to request the server to store the included body at a location specified by the given URL.                   |
| HEAD          | This method is same as that of a GET request, but without the response body and it transfers the header section only.                                                       |
| DELETE        | It will delete the specified resources.   |
| CONNECT       | It will establish the tunnel to the server identify by the resource.                                                   |
| OPTIONS       | It will describe communication options for the target resouce.                                                    |



---

<br/>
<br/>

# JAVASCRIPT
<br/>


## WHAT IS JAVASCRIPT?


* Javascript was created in 1995 BY THE Netscape Web Browser.

* Javascript is the language of the web,it is used to make the web look alive by adding motion to it. To be very precise,its a programming language that lets us implement complex and beautiful things or designs on webpages.

* Scripts are provided and exceuted as plain text.They don't need special preparation or compilation to run.

<br/>


## Javascript Datatypes:

<br/>

* **Primitive Datatypes** 
    1. Number 
    2. String
    3. Boolean 
    4. Undefined
    5. Symbol
    6. Null

* **Non-primitive Datatypes** 
    1. Object 
    2. Array
  

## Primitive DataTypes 

<br/>

### 1. Number
<br/>

```JS
3+4 = 7
(6+7)*2 = 26
12 % 6 = 0
12 % 5 = 2

"%" => Modulo - It gives us the Remainder.
```
<br/>

### 2. String 


<p><strong>String</strong> is just a text. all we need to do is let javascript know that we are writing a piece of text is in "Double-quote"</p>
<br/>

```JS
"Hello" + "there" = "Hellothere"
We can add strings.
"This isn't very nice" = "This isn't very nice"
'This isn't very nice' = Syntax cahnges,unexcepted idenitifier
'This isn\'t very nice' = 'This isn't very nice' 
['\] => This backslash has special meaning.It means whatever come after '\' is not piece of string.
```
<br/>

### 3. Boolean
<p>Boolean means just 'true' or 'false'. Somtimes that represents as 1's and 0's</p>

<br/>

```JS
3 > 2 = 'TRUE'
5 >=5 = 'FALSE' 
3 =3 = Uncaught syntax error: Invalid left hand side in assignment.
In javascript if we want to say something is equal to somthing then we have to say '==='.
now 3 === 3 = 'TRUE'
```
<br/>

### 4. Undefined
<p>As the name suggest this means that the variable has not been assigned</p>

<br/>

```JS
var b; = Undefined
var password = Undefined
```

<br/>

### 5. Symbol

<p> Javascript ES6(ECMAscript version 6) introduced a primitive data type called <strong>symbol</strong>. Symbols are immutable that means they can not changed</p>

<br/>

```JS
 const symbol1 = symbol();
 typeof(symbol1); // Symbol

 const sym2 = symbol("hello!");
 console.log(sym2); // symbol("hello!")
 sym2  // symbol("hello!")
 ```

<br/>

### 6. Null
<p>A NULL means absense of value. You can assign null to a variable to show that currently that variables does not have any value.</p>

<br/>

```js
var myPassword = null;
```
<br/>

## Non-Primitive Datatypes 

<br/>

### 1. Array
 
 <p><strong>Array</strong> is a variable that is used to store different elements. It is often used when we want to store list of elements.</p>

<br/>

 ```js
 var mixedList = ["apples","3","undefined","true","function apple(){
     console.log("apples")
 }];
 ```
```js
var list = [
    ["tiger","lion","mouse","bird"]
];

console.log(list);  // [Array(4)]
console.log(list[1]); //tiger
console.log(list[0][2]); //mouse
```

```js
// some of the operations we can perform on array.

var list = ["tiger","lion","mouse","bird"]
list.shift();//"tiger"
list // ["lion","mouse","bird"]

list.pop();
list //["lion","mouse"]

list.push("elephant");
list //["lion","mouse","elephant"]

list.conacat(["bee","deer"]);
list // ["lion","mouse","elephant","bee","deer"]

list.sort();
list // ["elephant","lion","mouse",] it will sort the original aaray beacause list.concat dont save into variable.

//now we have to concat the things we add afterward so will do like this :

var myList = ["lion","mouse","elephant","bee","deer"];
var myNewlist = myList.concat(["monkey"]);
myList //["lion","mouse","elephant","bee","deer"]
myNewlist //["lion","mouse","elephant","bee","deer"]

//NOTE : push(); pop(); dont create new list they just modify the existing list.

```

<br/>


 ### 2. Object
 <p><strong>Object</strong> is nothing but the collection of properties.
 objects are always in a key:value pair.</p>

<br/>

 ```js
 //eg1
 var user {
     name: "poonam",
     age : 23,
     hobby: "dancing",
     isMarries : false
 };

 //If we want to add something ,
 user.favFood : "chiken";

 //now if we again console log the we willl get that added property
 user
  var user {
     name: "poonam",
     age : 23,
     hobby: "dancing",
     isMarries : false,
     favFood : "chiken"
 };

 ```

 ```js
 //eg2
   var user {
     name: "poonam",
     age : 23,
     hobby: "dancing",
     isMarries : false,
    spells: ["shazam","boom","shuhhhsh"]
 };
user.spells
// (3) ["shazam","boom","shuhhhsh"]

user.spells[1]
"boom"

 ```

 ```js
 //eg3
 var list =[
     {
         userName : "pooh",
         passWord : "@1234"
     },
      {
         userName : "prashant",
         passWord : "@marvel"
     }


 ];
 // if we want to access the password in the first object or second object then we will do like this:
 // list[0].password => "@1234" 
 
 ```
<br/>


## Javascript Variables :

1. var
2. let
3. const

<br/>

**Rules**

 1. It needs to start with letter.
 2. It can end with the number.
 3. It can't start with a symbol.
 4. A variable also start with a '$' or '_'.
 5. Camelcasing should be there.


### 1. var
<p><strong>var</strong> is a type of javascript variable.Which is used to store the value.</p>
<p><strong>var</strong> declarations are globally scoped or fuction scoped.</p>
<p><strong>var</strong> variables can be re-decalred and updated within the same scope and won't get an error.</p>
<p><strong>var</strong> is hoisted to top of their scope.</p>

<br/>

```js
var username = "poonam@123";

 => "poonam@123"
 ```

<br/>

### 2. let
<p><strong>let</strong> is use for variable declaration.</p>
<p><strong>let</strong> is a block scope.Anything within curly {} braces called block. So variable declared in a block with let is only avaible for use within that block.</p>
<p>A variable declared with let can be updated within scope,but cannot be re-declared within the scope.</p>
<p><strong>let</strong> declaration are hoisted to the top.</p>
<br/>

```js
let age = 23";

 => 23
 ```

<br/>

### 3. const
<p><strong>const</strong> is use for maintain the constant values.</p>
<p><strong>const</strong> declaration are block scoped.It can only access within the block they were declared.</p>
<p><strong>const</strong> value remains same whithin its scope.It cannot be updated or re-declared.</p>
<p><strong>const</strong> object can not be updated but properties of the object can be updated.</p>
<p><strong>const</strong> declaration are hoisted to the top.</p>

<br/>

```js
const password = "@1234";

 => "@1234"
 ```

<br/>
<!-- let and const images -->
<p align="center"/><img src="Images\letandconst.png" width="550" />

<br/>
<br/>

## Javascript Logical Operators 

<br/>

1. AND **&&** 
2. OR **||**
3. NOT **!**

<br/>

### AND **&&**

<p><strong>AND</strong> operator represented with the the two ampersands.</p>
<p>If bothe the arguments are<strong>true</strong>,it returns true, otherwise <strong>false</strong>.</p>

<br/>

```JS
var firstName = "Bob";
var lastName  = "Marley";
if(firstName === "Bob" && lastName === "Marley"){
    alert("Hi Bob Marley"); // shows the popup
}

var lastName = "Smith";
 => Undefined

 ```
<br/>


### OR  **||**
<p><strong>OR</strong> operator represented with the the two vertical lines.</p>
<p>If any of its arguments are <strong>true</strong>,it returns true,otherwise it returns <strong>false</strong>.</p>

<br/>

```JS
if(firstName === "Billy" && lastName === "eilish"){
    alert("Hi Billy E."); // shows the popup
}
```

<br/>

### NOT **!**
<p><strong>NOt</strong> operator represented with an exclamation sign.</p>
<p> It returns the invert values.</p>

<br/>

```JS
if(!(name === "Bob")){
    alert("hi bob");
}
 !true => false
 !false => true
 ```
<br/>


## Javascript Conditions 
<br/>

1. if
2. if-else
3. else if
4. tenery operator
5. switch

<br/>

### 1. if 
<p><strong>if</strong> condition we use if we want to eexecute something based on some condition.</p>

<br/>

```js
var name = "billy";
if(name === "billy"){
    alert("Hi im billy");
}

name = "susy";
//now if we try to run the program no alert message will be there.
```
<br/>

### 2. else
<p><strong>else</strong> statement when we want to execute the code every time when if condition evaluates false.</p>


<br/>

```js
var name = "billy";
if(name === "billy"){
    alert("Hi im billy");
} else{
    alert("I dont know you!")
}
```
<br/>

### 3. else if
<p><strong>else-if</strong> consdition is use when we want multiple else condition after if statement.</p>

<br/>

```js
var name = "billy";
if(name === "billy"){
    alert("Hi im billy");
} else(name === "susy"){
    alert("I am susy!");
}else{
    alert("I dont know you!");
}
```

<br/>

### 4. tenray operator 
<p><strong>tenery</strong> operator is used to assigning value depending on the condition.</p>

<br/>

```js
syntax:
Condition ? Expression1 : Expression2
```
```js
var password = isUserValid(true)? "You may enter" : "Access Denied"
```

<br/>

### 5. switch

<p>When there is more than one different cases the we will go for the <strong>switch</strong>.</p>

<br/>

```js
function movCommand(direction){
    var whatHappens;
    switch(direction){
        case "forword":
        whatHappens = "You encounter the monster";
        break;
        case "backword":
        whatHappens = "You will be eaten by monster";
        break;
        case "right":
        whatHAppens = "Move to your right";
        break;
        case "left":
        whatHappens = "Move to your left";
        break;
        default:
        whatHappens = "Enter the valid expression";
        break;
    }
    return whatHappens;
}

// if you run this is console the,
//window.moveCommand("forword");
//=> "You encounter the monster"

```
<br/>

### Scopes in Javascript :

The Scope which manages the accessibility of variables.

<br/>

```js
const password = "@1234";
console.log(passsword); // "@1234"
```
```js
if(true){
    const password = "@1234";
}
console.log(passsword); //Referance error!

// The if  code block craete a scope for password variable and this variable can access only within this scope only. Within the scope we can console log it but outside the scope variable is not asccessible.
```
<br/>

**Block scope**
 <p> A block of code in Javascript defines a scope for variables declared using let and const.</p>

<br/>

 ```js
 if(true){

     //'block' scope
     const password = "@1234";
     console.log(password); // "@1234"
 }

    console.log(password); // we will get an Referance error!


//In the first console log will get the output beacause it  can be accessed where it it defined that is inside the scope.

// But hen we are concole logging from outside the if block then it will throw us an error.

// if,while,for these loops crete the block scopes and in this mostly let and const variables are used.
 ```

<br/>

**Function scope**

<p>A Function in a javascriptdefines a scope for vaeiables declared using var, let and const. </p>

<br/>

```js
function walk(){
    var msg = "walk in the forword direction";
    console.log(msg); // "walk in the forword direction"
}
console.log(msg); // Referance Error!!

// walk function creates a function scope. The variable msg is accessible inside of the function scope but not accessible outside the function scope.
```
<br/>

**Global scope** 
``` js 
1. The Global scope is the outermost scope. It is accessible form any inner scope.
2. window and document are the global variablles supplied by the browser.
```
<br/>

### <strong>Variables</strong> is referred as a container.
<br/>

<p align="center"/><img src="Images\container.png" width="550" />

</br>

</br>


### <strong>Hoisting</strong> in javascript means behaviour of a function or variable can be used before declaration
<br/>

<p align="center"/><img src="Images\Hoisting.png" width="550" />

<br/>


## Javascript loops 

<p><strong>Loops</strong> are the execution of set of iinstructions repeatedly while some condition evaluates to true.</p>

1. for loop
2. while loop
3. do while
4. forEach

### 1. for loop

<p><strong>for loop</strong> loops through the block of code until the conuter reaches to the specified number.</p>

<br/>


### 2. while loop

<p><strong>while loop</strong> loops through the block of code until the consdition reaches to the specified evaluates to true.</p>

<br/>


### 3. do while loop

<p><strong> do while loop</strong> loops through the block of code and then condition is evaluated.If the condition is true,the statement is repeated as long as the specified condition is true.</p>

<br/>

<p align="center"/><img src="Images\loops.png" width="550" />

<br/>

### 4. forEach
i. for of

ii. for in

<p><strong>forEach</strong> method is used to iterate over the elements of an array.</p>

<br/>

### i. for of
<p><strong>for of</strong> loops over iterable objects such as aarays,strings etc..</p>

<br/>

### i. for in
<p><strong>for in</strong> loops through the properties of an object.</p>

<br/>

<p align="center"/><img src="Images\loops2.png" width="550" />

<br/>
<br/>

## Javascript Functions 

<p>Without functions javascript wouldn't do anything. The beauty is thst functions can perform one action or multiple actions. eg. alert(),  prompt() </p>

<br/>

<!-- images of functions -->
<p align="center"/><img src="Images\Functions.png" width="550" />

<br/>
<br/>

### Arrow Functions

<br/>

 <p> Arrow function is one of the features introduced in ES6 of javascript.</p>
 <p>It allows us to create function in a cleaner way compare to the regular way.</p>
 <p>Arrow function have more concise syntax.</p>


<br/>

```js
const sum = function sum(a,b) {
    return a+b;
}
// In arrow function :
const sum = (a,b) => a+b ;
```

```js
//with no argument
function randomNumber() {
    return Math.random;
}

//arrow function
const randomNumber = () => Math.random;
```

```js
document.addEventListener ('click',function() {
    console.log('click)
});

//arrow function

document.addEventListener ('click',function() => console.log('click);
```

<br/>


### Callback Functions 

<p>Pasing a function into another funcation is called as the callback function.</p>

Suppose we have a button with the id of btn

<br/>

```html
<button id = "btn">Save</button>
```

```js
btn.addEventListener ("click", addListAfterClick);
btn.addEventListener ("keypress", addListAfterClick);


function addListAfterClick(){
    --code--
}

'''
1. This is called callback function. When this line of code runs in javascript,we dont want the addListAfterClick function to run beacause we are just addding the event listeners now to wait for a click or keypress.

2. We want to let it know this action to happen when a click or keypress happens. 

3. So the function now automatically gets run every time click happens, so we are pasing referance to the function without calling it.

'''
```

<br/>


## Pass By Value vs Pass By Reference 
<br/>


### **Pass By Value**
<p><strong>pass by value</strong>a function argumeents are always passed by value. It means that javascript copies the values of passing variables into arguments inside of the function.</p>

</br>

### **Pass By Reference** 
<p>In <strong>pass by reference</strong> instead of making a copy of the original,we are making a reference to the original value.So the change made on the reference is actually changing original.</p>
<p>In jvascript only arrays and objects follow <strong>pass by reference.</strong></p>

</br>

<!-- images -->
<p align="center"/><img src="Images\passbyvalue_1 (1).jpg" width="500" />

<p align="center"/><img src="Images\passbyreference_1 (1).jpg" width="500" />

<br/>


## **Reference Type** 
<p><strong>Reference type</strong> is a non-primitive type which are not defined by the programming lanuage.</p>
<p>Objects are what called the <strong>Reference type</strong> in javascript.</p>

<br/>

<p align="center"/><img src="Images\constructor (1).png" width="500" />


<br/>



## **Constructor** 
<p><strong>Constructor</strong> isna function which creates instance of object in javascript.</p>

<p align="center"/><img src="Images\constructor2.png" width="500" />

<br/>
<br/>
<br/>

## **Destructuring**

<p>Destructuring assignment take value from arrays or properties from objects and set them as aalocal variables. It is a technique that can make our javascript code more concise and readable.</p>

<br/>

```js
  // Object Destructuring
  const display =(person) =>{
      const{name,age} =person
      console.log(name); //Prashant
      console.log(age); //19

  }

  const display_2 = ({name:first-name,age}) =>{
      const name = "Poonam";
      console.log(first_name); //Prashant
      console.log(name); //Poonam
      console.log(age); //19
  }

  let person = {
      name:"Prashant",
      age:19,
      gender:"Male"
  }
```

<br/>

<p align="center"/><img src="Images\destructuring_1.jpg"  />


<p align="center"/><img src="Images\destructuring_1.jpg"  />