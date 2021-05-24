
# Basic building Block of Web Development
__________________________________________

## IP  : 
* IP stands for Internet Protocol.

* Internet protocol is the communications protocol that is address assigned to each device to connected to the network.

* Data is divided into the small pieces called 'Packet'.

<!-- image of Ip address  -->

<p align="center"/><img src="Images\web_1.jpg" width="500" />
<p align="center"/><img src="Images\web2_1.jpg" width="500" />


<!-- Ipv4 vs Ipv6 -->
<!-- Image -->
<p align="center"/><img src="Images\ipv4v6_1.jpg" width="500" />


<!-- Port Number -->
## Port Number :

* Port number related to to the network addressing.
*Port Number, which helps to get connected with a particular server.



 ### Server :

 <p> A server is a hardware and software devices which bascially take a request from thhe client or user and give it back to response.</p>

 ### Web server : 

 <p>Websites is a collection of web pages while web server is a software that respond to the request for the resources. </p>








<!-- HTTP Verbs -->
## HTTP Verbs : 


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
|               |                                           |





# JAVASCRIPT



## WHAT IS JAVASCRIPT?


* Javascript was created in 1995 BY THE Netscape Web Browser.

* Javascript is the language of the web,it is used to make the web look alive by adding motion to it. To be very precise,its a programming language that lets us implement complex and beautiful things or designs on webpages.

* Scripts are provided and exceuted as plain text.They don't need special preparation or compilation to run.



<!-- links -->

[Gradient Generator](https://github.com/poonam-channe06/Gradient-Generator)

[Gradient Generator](https://github.com/poonam-channe06/Gradient-Generator "Gradient-Generator")



## Javascript Datatypes:

* Primitive Datatypes :
1. Number 
2. String
3. Boolean 
4. Undefined
5. Symbol
6. Null

* Non-primitive Datatypes :
1. Object 
2. Array
  

## Primitive DataTypes : 
### 1] Number:

```JS
3+4 = 7
(6+7)*2 = 26
12 % 6 = 0
12 % 5 = 2

"%" => Modulo - It gives us the Remainder.
```
    
### 2] String :
<p>Its just a text. all we need to do is let javascript know that we are wrting a piece of text is "Double-quote"</p>

```JS
"Hello" + "there" = "Hellothere"
We can add strings.
"This isn't very nice" = "This isn't very nice"
'This isn't very nice' = Syntax cahnges,unexcepted idenitifier
'This isn\'t very nice' = 'This isn't very nice' 
['\] => This backslash has special meaning.It means whatever come after '\' is not piece of string.
```

### 3] Boolean : 
<p>Boolean means just 'true' or 'false'. Somtimes that represents as 1's and 0's</p>

```JS
3 > 2 = 'TRUE'
5 >=5 = 'FALSE' 
3 =3 = Uncaught syntax error: Invalid left hand side in assignment.
In javascript if we want to say something is equal to somthing then we have to say '==='.
now 3 === 3 = 'TRUE'
```


### 4] Undefined :
<p>As the name suggest this means that the variable has not been assigned</p>

```JS
var b; = Undefined
var password = Undefined
```

### 5] Symbol : 
<p> Javascript ES6(ECMAscript version 6) introduced a primitive data type called 'symbol'. Symbols are immutable that means they can not changed</p>

```JS
 const symbol1 = symbol();
 typeof(symbol1); // Symbol

 const sym2 = symbol("hello!");
 console.log(sym2); // symbol("hello!")
 sym2  // symbol("hello!")
 ```

### 6] Null :
<p>A NULL means absense of value. You can assign null to a variable to show that currently that variables does not have any value.</p>

```js
var myPassword = null;
```


## Non-Primitive Datatypes :

### 1] Array :
 
 <p>Array is a variable that is used to store different elements. It is often used when we want to store list of elements.</p>

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


 ### 2] Object :
 <p>Object is nothing but the collection of property.
 objects always in a key:value pair.</p>

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


## Javascript Logical Operators :

1. AND (&&) 
2. OR (||)
3. NOT (!)


### AND (&&):

```JS
var firstName = "Bob";
var lastName  = "Marley";
if(firstName === "Bob" && lastName === "Marley"){
    alert("Hi Bob Marley"); // shows the popup
}

var lastName = "Smith";
 => Undefined

 ````



### OR (| |);

```JS
if(firstName === "Billy" && lastName === "eilish"){
    alert("Hi Billy E."); // shows the popup
}
```



### NOT (!) :

```JS
if(!(name === "Bob")){
    alert("hi bob");
}
 !true => false
 !false => true
 ```



## Javascript Conditions :
1. if
2. if-else
3. else if
4. tenery operator
5. switch


### 1]  if :

```js
var name = "billy";
if(name === "billy"){
    alert("Hi im billy");
}

name = "susy";
//now if we try to run the program no alert message will be there.
```


### 2] if-else:

```js
var name = "billy";
if(name === "billy"){
    alert("Hi im billy");
} else{
    alert("I dont know you!")
}
```


### 3] else if:

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

### 4] tenray operator :

```js
syntax:
Condition ? Expression1 : Expression2
```
```js
var password = isUserValid(true)? "You may enter" : "Access Denied"
```


### 5] switch :

<p>When there is more than one different cases the we will go for the switch.</p>

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


### Scopes in Javascript :

* The Scope which manages the accessibility of variables.

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

* Block scope :
 <p> A block of code in Javascript defines a scope for variables declared using let and const.</p>

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


* Function scope :
<p>A Function in a javascriptdefines a scope for vaeiables declared using var, let and const. </p>

```js
function walk(){
    var msg = "walk in the forword direction";
    console.log(msg); // "walk in the forword direction"
}
console.log(msg); // Referance Error!!

// walk function creates a function scope. The variable msg is accessible inside of the function scope but not accessible outside the function scope.
```

*global scope :
``` js 
1. The Global scope is the outermost scope. It is accessible form any inner scope.
2. window and document are the global variablles supplied by the browser.
```
## Javascript Variables :

1. var
2. let
3. const

* Rules :
 1. It needs to start with letter.
 2. It can end with the number.
 3. It can't start with a symbol.
 4. A variable also start with a '$' or '_'.
 5. Camelcasing should be there.


### 1] var :
<p>It is a type of javascript variable.Which is used to store the value</p>

```js
var george : "These pretzelas are making me thirsty" + "!";

 => "These pretzelas are making me thirsty!"
 ```

<!-- let and const images -->
<p align="center"/><img src="Images\letandconst.png" width="550" />


## Javascript Functions :

#### <p>Without functions javascript wouldn't do anything. The beauty is thst functions can perform one action or multiple actions. eg. alert(),  prompt() </p>

<!-- images of functions -->
<p align="center"/><img src="Images\Functions.png" width="550" />

 *  Arrow Functions :
 <p> Arrow function is one oo the features introduced in ES6 of javascript.</p>
 <p>It allows us to create function in a cleaner way compare to the regular way.</p>
 <p>Arrow function have more concise syntax.</p>


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


* Callback Functions :
<p>Pasing a function into another funcation is called as the callback function.</p>

Suppose we have a button with the id of btn

```html
<button id = "btn">Save</button>
```
```js
btn.addEventListener ("click", addListAfterClick);
btn.addEventListener ("keypress", addListAfterClick);


function addListAfterClick(){
    --code--
}
```
```html
1. This is called callback function. When this line of code runs in javascript,we dont want the addListAfterClick function to run beacause we are just addding the event listeners now to wait for a click or keypress.
2. We want to let it know this action to happen when a click or keypress happens. 
3. So the function now automatically gets run every time click happens, so we are pasing referance to the function without calling it.
```



## PassByValue vs PassByReferance :
<!-- images -->
<p align="center"/><img src="Images\passbyvalue_1 (1).jpg" width="500" />

<p align="center"/><img src="Images\passbyreference_1 (1).jpg" width="500" />